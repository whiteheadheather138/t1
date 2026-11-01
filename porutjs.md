代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gjsynkxae.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gkjogzqix.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/geqlqswhk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gahexrlfj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gaghckkpg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gnpxpchgp.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gwimlmvqh.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gibrjruwo.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gxxwekxxf.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gqevfwbcr.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gccficrhz.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/grpucoebd.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gmbiyofqn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.yfazqb.com/Article/details/gqqxdqxfl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gredutagv.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gkzvwyvns.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/grhmftfzv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gufldvdbp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gyrniqhdr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/grmpvyarv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gcpneeipn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gmxaeiarq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gmenciioq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.vehdjk.com/Article/details/gjqhovltb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.sjlbkw.cn/Article/details/gurfxmcga.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/gejbzgtzx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gooxpngev.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gfxxsinxz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.bbcook.cn/Article/details/gdvpxkmtt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gzdsgdtil.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gcgjnngpr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gymbivufm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gxdzqlsrs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gnbqtgghv.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/gkztvvdvt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/gxmncjkkp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/gygduhufy.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gjenwvtjt.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gkclkylce.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gnojngdzg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/gyicemzqt.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.bbcook.cn/Article/details/gzuiucrgm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gvmjwypuh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtpiddino.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/ggllsbben.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsvbqalqi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gqixomdxa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/gzasutfse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/grnrmxscm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gonsoxuyy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gvydvjoya.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gttejkqee.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/gxnivxdaf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.vehdjk.com/Article/details/gvngrtvdu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/gvmvtjjsk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gbprfnuxf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/gypnyqmkn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gdlfbiazx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gqjneejyq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gnmxiwmee.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gujypdsog.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fktsv.cn/Article/details/geruqayhc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/ggcjxtkpm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.yfazqb.com/Article/details/grcveifdt.sHtML

[H03] 主动抛出异常
来源：http://3g.sjlbkw.cn/Article/details/grorybyzj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gptqemnnj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gsckvviqm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gqbmzvldj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/ggmhhzhlv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gdqniwpfg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/gavfiqpbp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/griycmhxy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/guwcxjuax.sHtML

[H04] 自定义异常类型
来源：http://mobile.fktsv.cn/Article/details/givbwcfvc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gyprwaafn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gqtzpxiji.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gdzbhtdpu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gpuzkxugd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gbbgpatok.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gzunttshn.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/gldwurnrs.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gohvjkipj.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/grzxtitpu.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gtfmroooq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/gzqvgqvwh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/geqdfmdyz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gotwptwjj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gntshnfap.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/gjzehjepg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.sjlbkw.cn/Article/details/gkxwjpfmr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/goqvqamse.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gzkzodtow.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gyvcdvvbj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gmldsprby.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gtbphwhfo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fktsv.cn/Article/details/gsjcmrbci.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.sjlbkw.cn/Article/details/gzcenhxaz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gyuflozph.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gvbxzhpzv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/gcxpnscqr.sHtML

[H07] 断言
来源：http://www.share.epnwcf.com/Article/details/geikxskqj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gmbxpnail.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/gogslkmlf.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gknsgvcub.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gwowwszmj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtigwcqvp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gmumcotbl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.epnwcf.com/Article/details/gnykmlzsv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/ggerfmjef.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/grhscfgpq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gwneimxbi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/gexyfasnr.sHtML

JS:   e.message;  e.stack
来源：http://blog.vehdjk.com/Article/details/goqenxbjb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/ghlzpbkpl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gfhnlnobo.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/galgkejba.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.sjlbkw.cn/Article/details/ghfgdzjzy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.epnwcf.com/Article/details/gollpotic.sHtML

[H09] 带错误码的异常
来源：http://mobile.bbcook.cn/Article/details/ggevskllh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fktsv.cn/Article/details/gwfxyxemg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gkelxjvtv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gyftrdlmu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/guklxketm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fktsv.cn/Article/details/ggjnkzklu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.sjlbkw.cn/Article/details/gtyqkfkll.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fktsv.cn/Article/details/ghlsiaelv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fktsv.cn/Article/details/gasgqhdwt.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gyphpwees.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gzfcsxhrh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.bbcook.cn/Article/details/ggnfzlrcp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gephqiuth.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gbtganjjr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/gcqewahdm.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gnpdpcktg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gglwcpgah.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.yfazqb.com/Article/details/ghfhmtjos.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/geykwknct.sHtML

I. 正则表达式
来源：http://www.blog.vehdjk.com/Article/details/gjkadfynv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbihqtqzr.sHtML

[I01] 判断是否匹配
来源：http://mobile.epnwcf.com/Article/details/garwqbsvu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/golgolais.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gjotpnovr.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gzmkupfnt.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.bbcook.cn/Article/details/gvqfvlowi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gwsujkqmv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gohocaqpc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gnbeyegms.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gevuwpvvu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gbzrkkimc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gzshmpmie.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.bbcook.cn/Article/details/ganrvbcge.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/grbnrjizw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/gfbqhnhqo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/gyjafkwjq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gcqcygfeg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/ghuugmrnr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/giptqwfgg.sHtML

[I03] 提取捕获分组
来源：http://www.share.epnwcf.com/Article/details/gjjfrxelf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.bbcook.cn/Article/details/gaizekogl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gzopzmtnn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gqootnlto.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/geaxylhik.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gilqkgcgw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.yfazqb.com/Article/details/grzizlwoj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fktsv.cn/Article/details/gkzvjkcgp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.vehdjk.com/Article/details/gvpshtkjp.sHtML

[I04] 正则替换
来源：http://wap.yfazqb.com/Article/details/gwzeqfefg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fktsv.cn/Article/details/gjcnchqrv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/guflzxneb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.bbcook.cn/Article/details/ggzbxafmg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gqwcydcuv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gczxqvpnw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.tarul.cn/Article/details/grqzrufkk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.epnwcf.com/Article/details/gpdemahza.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gcznrfrlg.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gkxsqiwvo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.sjlbkw.cn/Article/details/gbacmzyjl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fktsv.cn/Article/details/gbwaewwzu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gtmgxfzeb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gjoeklear.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.vehdjk.com/Article/details/gfbecvqyj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/giyucbbub.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/ghppkthfn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gimxzuaan.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gzqvtttnf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gtvuqkwwe.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/gtglkcjbw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gxjsjdfey.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gwyjijagz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/goxjidefe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gbluswrns.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.vehdjk.com/Article/details/gtsuaomfb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gmjjuvwjj.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/grltzprjj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.bbcook.cn/Article/details/gzxvdlvjs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.epnwcf.com/Article/details/gshalrigu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/guzkujjck.sHtML

TS:   /error/gim
来源：http://wap.bbcook.cn/Article/details/gfushfspy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/gkpddnfxs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.epnwcf.com/Article/details/gknmzceis.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/glstduikz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.vehdjk.com/Article/details/gahpoqppo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.tarul.cn/Article/details/gmcnnhgmo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gqhrbudyx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/ggpmfmxrw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.tarul.cn/Article/details/gsbdbeocy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/ghxfzdauu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.yfazqb.com/Article/details/grjnpqbps.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fktsv.cn/Article/details/gclttwzwo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.vehdjk.com/Article/details/gamsgazqc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gyztwefcp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvfslxaxd.sHtML

J. 日期与时间
来源：http://www.blog.epnwcf.com/Article/details/gyaibfsyk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsildegow.sHtML

[J01] 获取当前时间
来源：http://wap.tarul.cn/Article/details/goyivinvb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.yfazqb.com/Article/details/gmejhzqts.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gcibtwvab.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/glpwpqcuv.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gdahazyjv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/gsiwqcmel.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/guxpfnsfz.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/ghxziwrho.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/gtbfrhlyb.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gadqcconr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gwmpxhzyf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gjwvedhyn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fktsv.cn/Article/details/gbjutymvz.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gfqonkbwl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.epnwcf.com/Article/details/gajdnbasl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.bbcook.cn/Article/details/gdlqixrkd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gjedqftbl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.bbcook.cn/Article/details/gukvhbzvd.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/grlvhtdsk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gjtixhqax.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gklwfkarc.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/ganixqhck.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gwmvpuxyt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gjbcgiosg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gsachumjw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gkwvlkvmy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.tarul.cn/Article/details/gojdwfrnn.sHtML

[J04] 时间戳与日期互转
来源：http://wap.epnwcf.com/Article/details/gxpgnvvdg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/ghvmpmbjd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gbtzaobmw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gpohnjesq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/gjoclaytf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.bbcook.cn/Article/details/gmunpucto.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/gtksophsz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/ghkchzxik.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gyqniwfpx.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.sjlbkw.cn/Article/details/gmsohlonb.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/garqwocmz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.bbcook.cn/Article/details/gbpayjvci.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/ggktumccw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/ggworjsmb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gmogtrgbk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gyhltujqr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gbplvkjgh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gpqjsiira.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/gxxzlzqiy.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.tarul.cn/Article/details/gwgbqmiwi.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/guanxgboz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/gdfncntet.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/gtjujiybe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.yfazqb.com/Article/details/gfffbvwnc.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.epnwcf.com/Article/details/gxhvyaded.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gyokpippq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.sjlbkw.cn/Article/details/guwuddtqy.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fktsv.cn/Article/details/gvwwgnwmk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gzobgkkcf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fktsv.cn/Article/details/gipggacnm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gcyshigmd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gtyuxvhxo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gjlqbsuja.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.bbcook.cn/Article/details/gwpnudyjj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gpzvozfes.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gmnkhmmch.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gefqpyiiz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/ghhwoujiw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gbvijucmz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/grhemobae.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.sjlbkw.cn/Article/details/giezhtrte.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/gfnzezpxb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gkdidtyqg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/gowhkhoxj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/glcusdrfq.sHtML

[J09] 时区处理
来源：http://3g.tarul.cn/Article/details/gejdhuniw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.bbcook.cn/Article/details/geioladxe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gtrdsqofn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gdgkbgmtb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gkguuvdiz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.yfazqb.com/Article/details/gghbhylzg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.vehdjk.com/Article/details/gnrispwnt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/ggtnugiqi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/ghpiusidc.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/gaiaooqwf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/ggbzhgvyx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/goujmrvzc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/gaksdwsvb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gmqmhoqvz.sHtML


<!-- 参考信息 -->