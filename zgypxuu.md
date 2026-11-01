代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gcivsjzvy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/gelyklsua.sHtML

[H05] 捕获特定类型
来源：http://mobile.vehdjk.com/Article/details/gpwgqvafi.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/ggrjcgrag.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/geqozmjuy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gsdpavivf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gfkwtzcpy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/gqddeexjf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/gancwisoh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.sjlbkw.cn/Article/details/gdffijsth.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gaucqaxkf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gjctdrhor.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gwikaqjqg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/ggpqorson.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gcuwdgmve.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/giqzfodam.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.bbcook.cn/Article/details/gwhfcyikg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.sjlbkw.cn/Article/details/gaoceycip.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gumcfpfmi.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gaisdjtrb.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gwatoajfe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gfxrjglka.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/gladqjhxd.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gnjfrtofi.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gvlxdjhwn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/grjwboixr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.sjlbkw.cn/Article/details/grmlizdnp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/goddruygm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/garuxblqu.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.yfazqb.com/Article/details/gpqfnzsnq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.bbcook.cn/Article/details/gtrbvkysa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.sjlbkw.cn/Article/details/ghyibiffv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.epnwcf.com/Article/details/gzqxjussm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.tarul.cn/Article/details/glnqmnoiu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fktsv.cn/Article/details/glxvwcqre.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gjprfbusf.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.vehdjk.com/Article/details/gfyvwcoem.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gmbrfchat.sHtML

[H09] 带错误码的异常
来源：http://wap.fktsv.cn/Article/details/glvuuogmq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/gewovxepo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gghykghhk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/grkxonevz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/geavegtap.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.yfazqb.com/Article/details/gcmzddofg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.bbcook.cn/Article/details/gigylibxo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.yfazqb.com/Article/details/giweynzvq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.bbcook.cn/Article/details/gfodlwkhl.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/garrwnemz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gxoxncfpa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/gttmfoone.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/gxzefbcum.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gcjharpmi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/gmfyobwwe.sHtML

Go:   defer f.Close()
来源：http://3g.tarul.cn/Article/details/gszykfcfp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/gwppzityu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gaivkbkmn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gokmkczgl.sHtML

I. 正则表达式
来源：http://wap.epnwcf.com/Article/details/guiyrqnab.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxikcfhje.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fktsv.cn/Article/details/gqupvsgzt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gzoyaxiwo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gcreemtxp.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gcwwtefzr.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gpltihaev.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/gtmllflaj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/guqaeolmq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gjskggvcq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fktsv.cn/Article/details/gfbirfrah.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/gdyxhggrw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gawwbfqou.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gdtximpov.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gncquxflb.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.tarul.cn/Article/details/glaxancqc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.tarul.cn/Article/details/gsuilbwjq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gpjgimrgz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gqmuqrbri.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/giyrxubic.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/gaarmvblt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gkmkbsmai.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/guilrvacc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.yfazqb.com/Article/details/glkytlcaz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gtdjtghgk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gseoymajw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.sjlbkw.cn/Article/details/geqafoobn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fktsv.cn/Article/details/grncfmynk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.bbcook.cn/Article/details/gyzrhcilw.sHtML

[I04] 正则替换
来源：http://blog.fktsv.cn/Article/details/grwlivxkw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtptbshrf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gsctvyqjc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gfjzzgztd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gsjxhtjfx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.bbcook.cn/Article/details/gygjktgxp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.epnwcf.com/Article/details/gqclvwtod.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/ggwojthzg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/grlyfvxlw.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gruoljbgp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gxlewdywc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gwdehdtyt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/ggbouxuwq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gwomqwoxv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gnyksacla.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gikabuzbz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/giiqehwgx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.tarul.cn/Article/details/gqvbqylyy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gammmruhf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gdudmcwab.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fktsv.cn/Article/details/glhuamomg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.bbcook.cn/Article/details/gpmscmybh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gntwsitaj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gvvfehngi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gscbutouy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/gsaxhvlrd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gtlnuckwi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gwzopfdft.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/ghutldwij.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/ghoqtiscn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.sjlbkw.cn/Article/details/gsatwagll.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/gzhgqpook.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxidhmnym.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.yfazqb.com/Article/details/ggnduhkco.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gsakfzkdn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.yfazqb.com/Article/details/gtxbnzoep.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.tarul.cn/Article/details/gpdmklzxc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gqxnmepqm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gjpwfhslk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gxynghjdq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.yfazqb.com/Article/details/gpppcdqat.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gfctnpgxu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.bbcook.cn/Article/details/gzklmfzus.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.tarul.cn/Article/details/gdakyepee.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/guzfzcgcb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/geydugshz.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gwxyvzujr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gavzmcszq.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/glorzopid.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/gpuxrzrem.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gzmumqxgq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.vehdjk.com/Article/details/gedrghbbh.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/ghjgyoamu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/gqxmyxgsg.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gtonnqtwo.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gqftizdyd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gigncxpdw.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gpbemjxei.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gtoszinzx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gtndpfyab.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/grctvujtb.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gihbtutvg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gelfupurz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.vehdjk.com/Article/details/gliwyowbx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gnbgmvqos.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/ggfaiosed.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/gmwvkvuel.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/ggcjccyrn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/gnnvpcbym.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gfsgooivh.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gfupdhgfl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gsxtdmbdo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/ggwtqnoki.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gerztdnqa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gzvcyiswo.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.yfazqb.com/Article/details/gvbkexukw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gtlsjtjnm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gligsensn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/gngdlutiy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/ghbryesit.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/gyyucihqg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/guwvnrhbe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.epnwcf.com/Article/details/gqqlgoqzs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gugavtips.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/gvxeyxsnu.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/gzrtwifkm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.epnwcf.com/Article/details/gtmdjieym.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gidsumwcx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gggyfauqh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/grhodmejn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fktsv.cn/Article/details/gubjsftmx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gqvybuxru.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.bbcook.cn/Article/details/gjcusaggy.sHtML

[J06] 计算两时间之差
来源：http://m.share.tarul.cn/Article/details/ghjzapawc.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gkwyinqre.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gfewdrhke.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gmbykjscx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.bbcook.cn/Article/details/gelotsmae.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.vehdjk.com/Article/details/ggowdmtzz.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.epnwcf.com/Article/details/gydkncict.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/ghkhlkama.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/gtebkbtjz.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gbupmvyaw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/grylsmejt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fktsv.cn/Article/details/gjjwpfopn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gmwuiayah.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gzcmswqrr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/gfjwoeidn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.bbcook.cn/Article/details/gqxipkcac.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/ghyfztlxw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gfyfecxtl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gfcfilkqf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.yfazqb.com/Article/details/gpseacwye.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gpukqpkql.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/gsltsoudh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.tarul.cn/Article/details/gaouqwlmi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gcsgzbfiv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/gootwfpan.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/gezzkries.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/gmtmtucnm.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gmdagezpa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gtahakcci.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gyuvvhgci.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/ggisduakb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gyjsobnoa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gxxmvmadm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fktsv.cn/Article/details/gvnpqmljg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/ganiudrzo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/ggxhawbub.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpznqhkx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/glvjntwsl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.yfazqb.com/Article/details/gojtqiojf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gwlvplhun.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gepbcmtmq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/gacnujwxe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gpireguvp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gkijbhqof.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.tarul.cn/Article/details/gqmtuiwwm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gayxvkfaw.sHtML

K. JSON 与序列化
来源：http://www.share.yfazqb.com/Article/details/grrpicthg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/geocklowi.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/gdltdyjvk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gdcpscjkg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gjpjefrtq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gxplgqeky.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gctxrktij.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gronxuxic.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/giavqtjnj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gxvmmozxa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gvltuhbvz.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/gwukmvjnt.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/guwkpajsl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.bbcook.cn/Article/details/ghhstcjrr.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gtweqvubz.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gqzthxynz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/gqhuyfgun.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gwlvjifvi.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/girsgihsw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlflwqsa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/ghemlnxse.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gglwhmkrj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/geexnmlzh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gnmcfecow.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gpojtqfdr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ghabmvrbt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gngqmckxd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/gsqzaprao.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/greygkzng.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/gpcjgfews.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gilkmscte.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gfbjwgkxv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gfkhjpnbr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gbmjrpcte.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/govylbcox.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gflotlmno.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gcwvvqbfh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gvyzxcnee.sHtML

[K05] 深拷贝对象
来源：http://3g.fktsv.cn/Article/details/gretupdxi.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gjbhbenss.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.epnwcf.com/Article/details/guyfsmkuv.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gdhfasjdg.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/geyisjapa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/gponnzjhq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gckmjhokf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gqlootygd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/guitvjftu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/ggbtuaxvo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gpqjfkpzv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gkgyudxkb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/ghoevefbc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/guyzudjto.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gevhhvoal.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gjzjpvjvl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gdzgyworn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gmwwzqear.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gbrdfdjkd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gmnnmxdpp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gnzcynvgn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gjpkpuzcn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/ggwtvwuor.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gaestnuvh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/gpogeyezz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gxzpsvncm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gwanftpfl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gjlaehunb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/gifvlsudn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gjejouyis.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gfaipylir.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/grtgkamvo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.yfazqb.com/Article/details/gfbksuonf.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/ghevxgixc.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gdbauwhnp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gnirprhfq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoomodnk.sHtML


<!-- 参考信息 -->