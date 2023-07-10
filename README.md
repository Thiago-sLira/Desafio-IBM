<h1>Segundo</h1>

<p>A classe <code>Segundo</code> é responsável por gerenciar um processo seletivo de candidatos. Ela permite o registro de candidatos, a marcação de entrevistas, a verificação do status de candidatos, a desqualificação de candidatos e a aprovação dos candidatos qualificados.</p>

<h2>Uso</h2>

<p>A classe <code>Segundo</code> oferece os seguintes métodos públicos:</p>

<h3><code>iniciarProcesso(nome: String): int</code></h3>

<p>Registra um novo candidato no processo seletivo.</p>

<ul>
  <li><strong>Parâmetros:</strong></li>
  <ul>
    <li><code>nome</code> (String): O nome do candidato.</li>
  </ul>
  <li><strong>Retorna:</strong></li>
  <ul>
    <li><code>int</code>: O código de identificação do candidato registrado.</li>
  </ul>
</ul>

<h3><code>marcarEntrevista(codCandidato: int)</code></h3>

<p>Marca uma entrevista para o candidato com o código de identificação fornecido.</p>

<ul>
  <li><strong>Parâmetros:</strong></li>
  <ul>
    <li><code>codCandidato</code> (int): O código de identificação do candidato.</li>
  </ul>
</ul>

<h3><code>desqualificarCandidato(codCandidato: int)</code></h3>

<p>Remove um candidato do processo seletivo, desqualificando-o.</p>

<ul>
  <li><strong>Parâmetros:</strong></li>
  <ul>
    <li><code>codCandidato</code> (int): O código de identificação do candidato.</li>
  </ul>
</ul>

<h3><code>verificarStatusCandidato(codCandidato: int): String</code></h3>

<p>Verifica o status de um candidato com base em seu código de identificação.</p>

<ul>
  <li><strong>Parâmetros:</strong></li>
  <ul>
    <li><code>codCandidato</code> (int): O código de identificação do candidato.</li>
  </ul>
  <li><strong>Retorna:</strong></li>
  <ul>
    <li><code>String</code>: O status do candidato.</li>
  </ul>
</ul>

<h3><code>aprovarCandidato(codCandidato: int)</code></h3>

<p>Aprova um candidato qualificado no processo seletivo.</p>

<ul>
  <li><strong>Parâmetros:</strong></li>
  <ul>
    <li><code>codCandidato</code> (int): O código de identificação do candidato.</li>
  </ul>
</ul>

<h3><code>obterAprovados(): List&lt;String&gt;</code></h3>

<p>Obtém a lista de candidatos aprovados no processo seletivo.</p>

<ul>
  <li><strong>Retorna:</strong></li>
  <ul>
    <li><code>List&lt;String&gt;</code>: A lista de nomes dos candidatos aprovados.</li>
  </ul>
</ul>

<h2>Exceções</h2>

<p>A classe <code>Segundo</code> pode lançar as seguintes exceções:</p>

<ul>
  <li><code>Exception("Candidato já participa do processo.")</code>: Lançada ao tentar registrar um candidato que já está participando do processo seletivo.</li>
  <li><code>Exception("Candidato não encontrado")</code>: Lançada quando um código de candidato inválido é fornecido ou quando um candidato não existe.</li>
  <li><code>Exception("Candidato já está aprovado!")</code>: Lançada ao tentar aprovar um candidato que já está aprovado.</li>
  <li><code>Exception("Candidato não qualificado para aprovação!")</code>: Lançada ao tentar aprovar um candidato que não está qualificado.</li>
</ul>
