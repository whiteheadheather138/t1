代发 wailian999

PHP:  public static function f() {}
来源：http://ulk.yfazqb.com

JS:   static f() {}
来源：http://ceh.jianghu66.top

TS:   static f(): void {}
来源：http://hpq.zycfv.cn

Java: static void f() {}
来源：http://ucz.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kec.zhixingplan.top

Ruby: def self.f; end
来源：http://duq.sjlbkw.cn

C#:   public static void F() {}
来源：http://grc.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://rey.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://qob.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://puo.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lhz.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://joy.aizwys.cn

Java: interface Shape { double area(); }
来源：http://wmx.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://amv.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hrr.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://fpk.cashguo.top

[G10] 访问控制
来源：http://gam.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://owi.aizwys.cn

PHP:  public / protected / private
来源：http://hzc.ivvv.top

JS:   #private 字段；其余公开
来源：http://sdg.shangyingyoupin.top

TS:   public / protected / private
来源：http://nnn.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://owp.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rod.havefunace.top

Ruby: public / protected / private
来源：http://agk.tanke756.top

C#:   public / protected / private / internal
来源：http://vyj.yuanzhike.top

[G11] getter / setter
来源：http://eem.yongpay.top

Py:   @property 与 @x.setter
来源：http://ebk.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qhc.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://zgt.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://pld.ehwqpu.com

Java: public String getName() { return name; }
来源：http://qee.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dgl.guannengcc.top

Ruby: attr_accessor :name
来源：http://kgy.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://htw.shuidangran.top

[G12] 对象转字符串
来源：http://ggq.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://por.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://edf.cashguo.top

JS:   toString() { return this.name; }
来源：http://slu.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://xtq.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://cfb.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zkn.sweek.top

Ruby: def to_s; @name; end
来源：http://jix.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://jtg.nwbrower.top

[G13] 判断对象类型
来源：http://wpv.chenlongwang.top

Py:   isinstance(u, User)
来源：http://zlz.cucudq.cn

PHP:  $u instanceof User
来源：http://reu.dianchejie.cn

JS:   u instanceof User
来源：http://psx.dianchejie.cn

TS:   u instanceof User
来源：http://zar.hfpthk.cn

Java: u instanceof User
来源：http://qsh.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rrw.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://izk.hywenlv.cn

C#:   u is User
来源：http://rty.yj20258888.top

[G14] 数据类 / record
来源：http://uky.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xbv.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://hec.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://rej.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://vqq.yonumen.top

Java: record User(String name, int age) {}
来源：http://rld.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://utf.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yvm.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://vlr.cheryme.top

[G15] 枚举
来源：http://dhc.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mcn.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jsi.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rsy.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://elk.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://lfi.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hld.hywenlv.cn

Ruby: Color = %i[red green].freeze
来源：http://qhj.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hwp.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://aqg.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wht.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://rmq.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://evw.cheryme.top

TS:   Object.entries(obj)
来源：http://cun.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ijy.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tny.xuanzx.com

Ruby: obj.instance_variables
来源：http://kuc.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://pyr.hysaishi.cn

================================================================================
来源：http://jeb.chenlongwang.top

H. 异常与错误处理
来源：http://nqq.sweek.top

================================================================================
来源：http://sgb.ydzc1.top

[H01] try / catch 基础
来源：http://uvi.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kwc.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yoo.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cwf.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nuo.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zys.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://giw.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xbe.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://asj.uphjek.com

[H02] finally / ensure 收尾
来源：http://ten.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://lgo.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://egf.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uia.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://kcv.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://aoq.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://whl.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gix.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ztf.zhengqikj.top

[H03] 主动抛出异常
来源：http://tzc.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://ssf.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jkp.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://fvw.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://qcp.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jbf.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ren.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gqe.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pcy.zdbjq.cn

[H04] 自定义异常类型
来源：http://cgy.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://pxd.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://saa.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://boj.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://dvq.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://kez.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lbo.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://eyt.tarul.cn

C#:   class MyException : Exception {}
来源：http://ixw.ctjpmb.com

[H05] 捕获特定类型
来源：http://kxb.yueranfly.top

Py:   except ValueError as e:
来源：http://ocx.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://laj.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://ihp.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://hdh.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://wmw.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://igl.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://ewp.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lfs.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://dap.xziqi.cn

Py:   value = d.get("k") or default
来源：http://gdj.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cej.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://mhn.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uls.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rpy.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uxq.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://yxu.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://icv.feifeiyinyue.top

[H07] 断言
来源：http://rse.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://quo.dashuyun.cn

PHP:  assert($x > 0);
来源：http://zhm.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://ziw.redwolf501.top

TS:   console.assert(x > 0);
来源：http://ogi.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://uxk.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jnr.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://zbn.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://dwj.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://ohj.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://twn.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://brg.fehbvm.com

JS:   e.message;  e.stack
来源：http://mkq.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://xun.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cuy.xuetiantiany.cn

Go:   err.Error()
来源：http://dwa.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://jih.hywenlv.cn

C#:   e.Message;  e.StackTrace
来源：http://hmz.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://qty.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://imu.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pwi.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mvo.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zop.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sjp.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cym.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://qoa.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dlm.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://gbt.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ufr.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vug.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kmj.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qsg.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://teh.xuanzx.com

Go:   defer f.Close()
来源：http://bly.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hyf.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ijk.birdmap.top

================================================================================
来源：http://ngg.nwbrower.top

I. 正则表达式
来源：http://mdh.birdmap.top

================================================================================
来源：http://jws.xziqi.cn

[I01] 判断是否匹配
来源：http://rem.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fsb.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qzy.uphjek.com

JS:   /\d+/.test(s)
来源：http://xgz.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://uou.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vbi.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kdl.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://osc.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tfy.yj20258888.top

[I02] 提取所有匹配
来源：http://zzf.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://vjc.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wzp.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://njl.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://drt.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nxg.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zsp.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://sjk.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://trb.uphjek.com

[I03] 提取捕获分组
来源：http://xbo.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ybr.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pxl.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sfo.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lct.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://byo.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://enq.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://plm.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pps.jqgufenzy.top

[I04] 正则替换
来源：http://tyn.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jxn.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jek.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pnx.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nhs.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://azw.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vys.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://koy.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eaf.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://xdy.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://rbn.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ydk.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://ngx.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://jmp.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://rhv.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://txf.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://zrd.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hnc.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xvh.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oub.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qyk.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tor.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jvr.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wek.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jeu.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xkf.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nbz.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://ivj.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wry.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wrt.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mdl.yangfankeji.com

TS:   /error/gim
来源：http://pmc.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://and.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vsq.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://vxg.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ais.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://xbi.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ahm.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gmn.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dsz.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mit.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://skx.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mun.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gol.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cke.xylfe.cn

================================================================================
来源：http://gsz.chenlongwang.top

J. 日期与时间
来源：http://agf.yuanzhike.top

================================================================================
来源：http://hsv.wangdashe.top

[J01] 获取当前时间
来源：http://cxh.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hkw.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jnb.epnwcf.com

JS:   new Date();  Date.now()
来源：http://krf.yueranfly.top

TS:   new Date();  Date.now()
来源：http://ewt.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nkz.cqqwz.cn

Go:   time.Now()
来源：http://pxo.yvedp.cn

Ruby: Time.now
来源：http://wyl.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dlr.chenjidiqi.icu

[J02] 格式化输出
来源：http://eqs.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://puv.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wip.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kqa.nanxuanxn.top

TS:   d.toISOString()
来源：http://apl.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wfr.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vka.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wru.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kyw.jqgfzy.top

[J03] 字符串解析为日期
来源：http://yyn.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hed.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xjt.yonumen.top

JS:   new Date("2024-01-02")
来源：http://ipy.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://fuv.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://yjz.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xgq.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://asg.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nfl.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://tna.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ayk.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bwv.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wyj.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fmi.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aqv.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mgx.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zzb.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://csw.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://laa.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://wjt.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://unj.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wmw.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cnn.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://bdk.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nqv.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://naa.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://gns.bjfxy.top

[J06] 计算两时间之差
来源：http://dxz.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://jxi.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://thv.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nlw.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lqv.zhijiandao.cn


<!-- 参考信息 -->