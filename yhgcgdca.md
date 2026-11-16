代发 wailian999

Ruby: attr_accessor :name
来源：http://prp.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://sbb.ydjk.org.cn

[G12] 对象转字符串
来源：http://nhi.sweek.top

Py:   def __str__(self): return self.name
来源：http://ura.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ovs.316326.xyz

JS:   toString() { return this.name; }
来源：http://gen.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://utm.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://fie.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://kem.zycfv.cn

Ruby: def to_s; @name; end
来源：http://xor.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://mog.shuidangran.top

[G13] 判断对象类型
来源：http://pjb.meibo888.top

Py:   isinstance(u, User)
来源：http://owi.zhengqikj.top

PHP:  $u instanceof User
来源：http://ysj.iojbl.cn

JS:   u instanceof User
来源：http://ekv.jlsjyb.cn

TS:   u instanceof User
来源：http://epl.zdbjq.cn

Java: u instanceof User
来源：http://wge.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lbw.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://eek.guannengcc.top

C#:   u is User
来源：http://ziy.zhongyouzk.top

[G14] 数据类 / record
来源：http://jqr.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nqs.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://kog.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://vuh.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://cpv.xinyue.icu

Java: record User(String name, int age) {}
来源：http://aih.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://dwl.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kas.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://fiz.yonumen.top

[G15] 枚举
来源：http://aml.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zpk.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wkf.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pbc.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://afn.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://svd.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dyb.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://rxs.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zji.316326.xyz

[G16] 对象转数组 / 字典
来源：http://rnq.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tjh.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://xfw.jianghu66.top

JS:   Object.entries(obj)
来源：http://jxy.hfpthk.cn

TS:   Object.entries(obj)
来源：http://ouv.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bwx.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fqv.yangfankeji.com

Ruby: obj.instance_variables
来源：http://rnw.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://cuf.havefunace.top

================================================================================
来源：http://qva.xziqi.cn

H. 异常与错误处理
来源：http://qvy.52xcode.cn

================================================================================
来源：http://rnd.uphjek.com

[H01] try / catch 基础
来源：http://ibp.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rlg.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dkk.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rqh.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uzs.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ufl.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zzc.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jzm.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ybw.meibo888.top

[H02] finally / ensure 收尾
来源：http://fvc.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://aau.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://huu.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yzz.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ntw.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://uzz.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dyr.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://viq.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://byc.xinyue.icu

[H03] 主动抛出异常
来源：http://psy.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://nas.shanyushiyangtech.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dmu.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://qjt.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://qxf.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xcn.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sqp.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gzk.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://dad.ydzc1.top

[H04] 自定义异常类型
来源：http://evy.tarul.cn

Py:   class MyError(Exception): pass
来源：http://esj.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://ebp.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://qkr.bjfxy.top

TS:   class MyError extends Error {}
来源：http://boe.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://mbf.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://djx.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://xuc.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://izn.jinqigfzy.top

[H05] 捕获特定类型
来源：http://ind.cdnleiting.top

Py:   except ValueError as e:
来源：http://ucy.kuanghao11.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xdj.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://dev.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://hlg.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://pbo.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yqh.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://vss.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qop.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://fqx.havefunace.top

Py:   value = d.get("k") or default
来源：http://miu.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://nrd.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://vrc.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rii.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rpr.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yrq.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://lrg.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://owb.birdmap.top

[H07] 断言
来源：http://jro.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://cvx.sysykeji.top

PHP:  assert($x > 0);
来源：http://bkl.316326.xyz

JS:   console.assert(x > 0);
来源：http://chj.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://uqh.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://asa.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yed.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://voa.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://vzs.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://igi.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://hrg.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dgg.ctjpmb.com

JS:   e.message;  e.stack
来源：http://nei.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://coj.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dnj.cheryme.top

Go:   err.Error()
来源：http://zpb.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://bkb.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://bza.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://gue.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cwb.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://fwh.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vhz.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fnk.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ouv.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ort.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://kzq.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gsu.zycfv.cn

[H10] 资源自动释放
来源：http://cnz.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://vyd.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lxq.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dcp.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lbd.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rky.yonumen.top

Go:   defer f.Close()
来源：http://wax.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ruw.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pgx.9152youxi.cn

================================================================================
来源：http://mgn.yvedp.cn

I. 正则表达式
来源：http://jjz.zhaomingkeji.xyz

================================================================================
来源：http://hvg.zdqjudy.top

[I01] 判断是否匹配
来源：http://aqt.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://prw.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://azn.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://lpr.xziqi.cn

TS:   /\d+/.test(s)
来源：http://psa.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ltq.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lhp.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://zsm.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nks.xuanzx.com

[I02] 提取所有匹配
来源：http://deu.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://dfy.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jsm.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://btz.uphjek.com

TS:   s.match(/\d+/g)
来源：http://ynh.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ufn.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vbv.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://ayn.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nse.sxryk.cn

[I03] 提取捕获分组
来源：http://dwb.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qva.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lnu.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oyx.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://quj.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wdt.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://emz.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://plx.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://goc.ywan-chungtsiang.top

[I04] 正则替换
来源：http://xie.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vaw.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mdq.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ibj.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uon.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://wrv.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dmn.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://wwk.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pdo.nwbrower.top

[I05] 按正则拆分
来源：http://bas.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ibp.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bxm.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://htb.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://vrl.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://iiq.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zip.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gti.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hcd.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://olf.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://otw.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://paw.sxryk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tbt.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkf.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://apk.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mpn.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://psm.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wqb.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://zue.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mbg.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dlh.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ksi.hnxiangtu.top

TS:   /error/gim
来源：http://klw.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lwq.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jew.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://ajl.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uoz.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://snt.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rax.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxs.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xki.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fjx.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dhl.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jig.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mfz.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vlx.tian-w.cn

================================================================================
来源：http://pno.cashguo.top

J. 日期与时间
来源：http://rwl.xylfe.cn

================================================================================
来源：http://qpq.hysaishi.cn

[J01] 获取当前时间
来源：http://yao.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ztr.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sgm.hammf.cn

JS:   new Date();  Date.now()
来源：http://fbu.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://wlx.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ybs.sxryk.cn

Go:   time.Now()
来源：http://gfj.aizwys.cn

Ruby: Time.now
来源：http://fky.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kso.quarkkingdee.top

[J02] 格式化输出
来源：http://ibj.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lar.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://saz.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ozn.zhengqikj.top

TS:   d.toISOString()
来源：http://hxh.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dzn.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ray.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gjo.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iri.snrcjt.cn

[J03] 字符串解析为日期
来源：http://nkj.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ovl.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cfm.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://mqn.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://gya.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://tsk.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tts.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://dws.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://met.cashguo.top

[J04] 时间戳与日期互转
来源：http://tlv.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://chi.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uml.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ith.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qcy.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wac.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iet.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tlg.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nck.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://ywm.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://ytu.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fzx.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvt.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dug.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://htd.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rdc.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://vyb.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pbs.fzhhl.top

[J06] 计算两时间之差
来源：http://ifz.cheryme.top

Py:   (end - start).total_seconds()
来源：http://pip.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://kaq.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bjv.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ynr.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://oih.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://imp.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://tli.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://yjk.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://uni.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://cvx.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xkg.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zez.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://vri.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://czb.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ehk.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://mqj.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://fow.xuanzx.com

[J08] 提取年月日与星期
来源：http://tdj.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hoz.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bre.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wbe.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nol.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vnb.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uhe.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yno.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://big.hnxiangtu.top

[J09] 时区处理
来源：http://qjb.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cyk.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hpo.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xch.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://loh.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rru.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fxz.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fwn.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://egk.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://blm.daria6918.cn


<!-- 参考信息 -->