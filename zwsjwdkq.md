代发 wailian999

Ruby: attr_accessor :name
来源：http://wzx.sweek.top

C#:   public string Name { get; set; }
来源：http://cqe.zhoulong.xyz

[G12] 对象转字符串
来源：http://mye.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://yiz.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fzy.nwbrower.top

JS:   toString() { return this.name; }
来源：http://znf.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://jjp.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://ecu.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nzw.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://lxx.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://ade.andypj.xyz

[G13] 判断对象类型
来源：http://itw.0kj1m.cn

Py:   isinstance(u, User)
来源：http://wow.tian-w.cn

PHP:  $u instanceof User
来源：http://tlu.bbcook.cn

JS:   u instanceof User
来源：http://xke.316326.xyz

TS:   u instanceof User
来源：http://ffj.wangshuangyany.cn

Java: u instanceof User
来源：http://yqq.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rrk.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://tzv.guowangkeji.top

C#:   u is User
来源：http://rtj.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://cki.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mkq.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://zim.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://wpd.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://xjd.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://wvj.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://div.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vou.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://msy.vqdsnc.cn

[G15] 枚举
来源：http://uca.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kgk.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tuo.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vqp.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hqi.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://iuc.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uuq.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://zzd.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://skp.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://mqt.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wge.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://fqt.cheryme.top

JS:   Object.entries(obj)
来源：http://ftl.hywenlv.cn

TS:   Object.entries(obj)
来源：http://kmn.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tbl.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xhh.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://qzb.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://eaf.9152youxi.cn

================================================================================
来源：http://lpm.jinqigfzy.top

H. 异常与错误处理
来源：http://rvs.xuetiantiany.cn

================================================================================
来源：http://lez.zhixingplan.top

[H01] try / catch 基础
来源：http://rmr.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ssw.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://byj.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xxc.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wdt.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pak.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nlu.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ldn.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zwa.tanke756.top

[H02] finally / ensure 收尾
来源：http://nuc.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://xax.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dzv.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://coz.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oba.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://whp.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mga.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://goq.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qhn.fehbvm.com

[H03] 主动抛出异常
来源：http://zja.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://yxn.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xtv.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://fsk.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://pkm.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uve.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vns.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xyn.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://znz.svipenyu.cn

[H04] 自定义异常类型
来源：http://exn.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://ngd.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://bka.aizwys.cn

JS:   class MyError extends Error {}
来源：http://wwx.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://obr.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://swc.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xed.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://nru.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://gjl.fzhhl.top

[H05] 捕获特定类型
来源：http://vbx.hesvh.cn

Py:   except ValueError as e:
来源：http://taf.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://raz.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://mmw.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://yej.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://wdp.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nps.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://biq.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jwa.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://eia.epnwcf.com

Py:   value = d.get("k") or default
来源：http://efu.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://bgj.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://qzf.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://gyq.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ghs.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tnj.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://vta.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://pbh.zhaomingkeji.xyz

[H07] 断言
来源：http://xct.jinqigufen.top

Py:   assert x > 0, "必须为正"
来源：http://zqe.hfpthk.cn

PHP:  assert($x > 0);
来源：http://tnk.52xcode.cn

JS:   console.assert(x > 0);
来源：http://jka.xuanzx.com

TS:   console.assert(x > 0);
来源：http://yjl.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://muz.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uew.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fnt.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://uav.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://ivc.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://gdu.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fso.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://xbf.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yps.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kpc.jianghu66.top

Go:   err.Error()
来源：http://bli.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://fgn.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://xyw.cdnleiting.top

[H09] 带错误码的异常
来源：http://vby.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://twq.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uka.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ghx.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yyc.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wfk.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://esg.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vry.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://phb.aizwys.cn

[H10] 资源自动释放
来源：http://txa.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qop.ivvv.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dqe.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qye.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nml.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://onp.fengsongda.top

Go:   defer f.Close()
来源：http://yzu.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zek.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nqs.shanyushiyangkeji.top

================================================================================
来源：http://bsl.ivvv.top

I. 正则表达式
来源：http://hgb.ppjwa.cn

================================================================================
来源：http://zzz.c1oappe.top

[I01] 判断是否匹配
来源：http://cdw.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tni.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://fwd.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://alq.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://joe.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ldt.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pyq.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://moe.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ude.yonumen.top

[I02] 提取所有匹配
来源：http://wnm.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://vyh.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jlo.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lpu.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://ibf.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gjv.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qrh.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://amd.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ndp.havefunace.top

[I03] 提取捕获分组
来源：http://ilj.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mss.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://isw.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tpn.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://glh.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ese.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hqa.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ima.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jan.zhiwuduotai.top

[I04] 正则替换
来源：http://cwr.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://cpk.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bhv.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://pjr.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://obd.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://pmd.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://evr.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oiq.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://btb.chenjidiqi.icu

[I05] 按正则拆分
来源：http://qdo.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://trn.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xfn.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://dfx.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://lca.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://oaq.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wdu.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://usd.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://szt.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xwp.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ulo.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://scn.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yha.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxr.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ohz.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ugj.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://njt.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ybw.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://jfd.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xlk.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zrh.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kty.zhaomingkeji.xyz

TS:   /error/gim
来源：http://jpe.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vjh.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vmk.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://vwl.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yug.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://xeu.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dqf.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iks.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wdk.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://unj.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://nvg.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hxc.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qpa.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nbi.gzhubu.top

================================================================================
来源：http://mjt.mhx1999.top

J. 日期与时间
来源：http://mpg.jyoumei.cn

================================================================================
来源：http://ghp.gotoacloud.top

[J01] 获取当前时间
来源：http://rzs.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rog.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yrp.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://xyp.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://uyt.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jmf.chenlongwang.top

Go:   time.Now()
来源：http://jln.uphjek.com

Ruby: Time.now
来源：http://lrg.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gsj.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://dcr.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nnu.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aat.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uyv.yanxiufei.cn

TS:   d.toISOString()
来源：http://dmk.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ick.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ojm.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://isc.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://icx.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://sul.yj20258888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vwa.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nnc.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://mqa.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://zld.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nvc.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nvt.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://kku.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qiz.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://dqv.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yhw.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oaj.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ojv.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gef.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gzg.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nqi.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qma.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ppa.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://yud.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://idg.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://eqd.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cxb.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yxo.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://hfd.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fzr.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://wnn.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mps.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://tid.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://rof.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://yfj.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zhz.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pdf.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://omm.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://kjj.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://xvo.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://ydi.nanxuanxn.top

[J07] 比较两个日期
来源：http://crq.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://iey.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://unx.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://bbr.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sqq.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gcs.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gtb.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://klq.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://dfh.sysykeji.top

[J08] 提取年月日与星期
来源：http://jft.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iyv.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://toe.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://enp.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eay.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rms.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pfq.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://avm.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oid.xuanzx.com

[J09] 时区处理
来源：http://zro.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zvd.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sda.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qwk.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hev.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vvl.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jme.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zue.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ywq.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://upf.gzhubu.top


<!-- 参考信息 -->