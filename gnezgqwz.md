代发 wailian999

Ruby: super
来源：http://rws.ydzc1.top

C#:   base.Greet();
来源：http://kpz.cucudq.cn

[G08] 静态方法与属性
来源：http://tej.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zcx.cucudq.cn

PHP:  public static function f() {}
来源：http://ijt.ehwqpu.com

JS:   static f() {}
来源：http://nws.ydjk.org.cn

TS:   static f(): void {}
来源：http://lgf.yj20258.top

Java: static void f() {}
来源：http://tbh.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ftg.wangdashe.top

Ruby: def self.f; end
来源：http://qbk.hongshengwenyu.top

C#:   public static void F() {}
来源：http://xjv.yfazqb.com

[G09] 接口 / 抽象类
来源：http://zbu.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://bgx.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://whu.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://atp.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://pyr.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://afh.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://bpg.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xqx.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://edr.snrcjt.cn

[G10] 访问控制
来源：http://xdm.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://nxf.sjlbkw.cn

PHP:  public / protected / private
来源：http://yir.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://kyq.hywenlv.cn

TS:   public / protected / private
来源：http://dyb.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://gcm.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://fxm.cashguo.top

Ruby: public / protected / private
来源：http://rjr.xylfe.cn

C#:   public / protected / private / internal
来源：http://afk.cdnleiting.top

[G11] getter / setter
来源：http://vhj.iojbl.cn

Py:   @property 与 @x.setter
来源：http://xlx.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ynb.tarul.cn

JS:   get name() { return this._name; }
来源：http://cot.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://kum.birdmap.top

Java: public String getName() { return name; }
来源：http://ctq.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hcr.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://juq.jianghu66.top

C#:   public string Name { get; set; }
来源：http://ebl.quarkkingdee.top

[G12] 对象转字符串
来源：http://vgw.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://abc.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xsc.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://dec.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://aqu.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://ykz.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hqj.sweek.top

Ruby: def to_s; @name; end
来源：http://zwb.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://yrt.meibo888.top

[G13] 判断对象类型
来源：http://ssh.bjfxy.top

Py:   isinstance(u, User)
来源：http://ezf.tianlin.xyz

PHP:  $u instanceof User
来源：http://qut.hysaishi.cn

JS:   u instanceof User
来源：http://fco.zhoulong.xyz

TS:   u instanceof User
来源：http://buj.shuidangran.top

Java: u instanceof User
来源：http://yel.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ysu.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://kzn.havefunace.top

C#:   u is User
来源：http://ggt.havefunace.top

[G14] 数据类 / record
来源：http://inp.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lrj.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://nno.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://tpt.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://kby.smart0.xyz

Java: record User(String name, int age) {}
来源：http://jbu.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://ppx.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ada.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://tkv.fktsv.cn

[G15] 枚举
来源：http://mxt.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://der.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hlf.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://euo.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dfi.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://lph.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://buf.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://zvy.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tjw.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://sur.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gft.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://exd.nwbrower.top

JS:   Object.entries(obj)
来源：http://bof.yonumen.top

TS:   Object.entries(obj)
来源：http://slu.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://umm.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ygb.ydzc1.top

Ruby: obj.instance_variables
来源：http://din.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://tld.hnxiangtu.top

================================================================================
来源：http://kfb.hammf.cn

H. 异常与错误处理
来源：http://mpc.pycfn.com

================================================================================
来源：http://xnu.xuanzx.com

[H01] try / catch 基础
来源：http://wdo.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://egc.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://myf.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://smq.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uaw.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pdk.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cfm.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qan.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fcs.sysykeji.top

[H02] finally / ensure 收尾
来源：http://ika.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://aef.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jzy.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eja.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bme.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://tcd.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gud.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rja.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jxr.yangfankeji.com

[H03] 主动抛出异常
来源：http://vvo.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://yly.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bmw.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://vhz.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://nbo.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qgh.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lfb.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mje.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rze.shzxlz.cn

[H04] 自定义异常类型
来源：http://jpq.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://cvb.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://atk.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://uzp.yj20258888.top

TS:   class MyError extends Error {}
来源：http://dic.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://lyu.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajx.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://vny.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://oev.xylfe.cn

[H05] 捕获特定类型
来源：http://hgy.sufxvd.cn

Py:   except ValueError as e:
来源：http://xjl.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nyx.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://lqc.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://jxw.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://mhq.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qkg.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://rfn.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://whj.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://sxa.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://aky.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://wce.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cuq.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://kbb.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jui.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vlm.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://jgs.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://met.sufxvd.cn

[H07] 断言
来源：http://pem.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://fyw.vehdjk.com

PHP:  assert($x > 0);
来源：http://kvs.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://srs.xylfe.cn

TS:   console.assert(x > 0);
来源：http://voi.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://dkk.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eaj.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://vtl.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://ygk.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://cga.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://dei.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://chc.fzhhl.top

JS:   e.message;  e.stack
来源：http://ppb.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fye.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://ckz.jinqigufen.top

Go:   err.Error()
来源：http://qfz.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://mhz.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://gbo.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://ehm.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fgk.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kgt.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ghs.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qcz.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pzy.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oih.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://hzf.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mjx.jqgfzy.top

[H10] 资源自动释放
来源：http://oun.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pzl.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cyb.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wns.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xln.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jia.zhengqikj.top

Go:   defer f.Close()
来源：http://oyd.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cae.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zou.nanxuanxn.top

================================================================================
来源：http://vze.aizwys.cn

I. 正则表达式
来源：http://kcc.jinqigufen.top

================================================================================
来源：http://fbd.yj20258.top

[I01] 判断是否匹配
来源：http://lmz.aibaodan.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hgv.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://pzz.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://zzy.c1oappe.top

TS:   /\d+/.test(s)
来源：http://zrz.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uvm.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dsm.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://bzg.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ogh.sufxvd.cn

[I02] 提取所有匹配
来源：http://ptn.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://wwy.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rfa.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ggz.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://frj.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hgq.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ufo.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://nfa.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ydp.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://zjw.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://msh.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tey.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dmo.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zsd.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://prw.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qeu.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://enb.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bqm.smart0.xyz

[I04] 正则替换
来源：http://xbo.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://yhp.yanxiufei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gou.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://rqy.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://mbu.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://zrq.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iqk.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dzw.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qek.iojbl.cn

[I05] 按正则拆分
来源：http://whz.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fbm.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ogm.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://kte.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://uji.xziqi.cn

Java: s.split("\\s*,\\s*")
来源：http://jbt.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oes.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://teq.mhx1999.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mto.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bzu.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://smf.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rnz.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://btn.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lek.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://khu.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://buj.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zwg.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tdf.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://zpv.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wfa.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nys.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fhs.hongshengwenyu.top

TS:   /error/gim
来源：http://iqv.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hww.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nwd.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://ppa.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qdv.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://kgi.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vvm.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tup.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pju.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lrs.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ufb.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ryg.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oxn.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qnh.nanxinkj.top

================================================================================
来源：http://byc.ctjpmb.com

J. 日期与时间
来源：http://gek.feifeiyinyue.top

================================================================================
来源：http://siy.xinyue.icu

[J01] 获取当前时间
来源：http://xfm.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ync.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xqs.redwolf501.top

JS:   new Date();  Date.now()
来源：http://hfl.cheryme.top

TS:   new Date();  Date.now()
来源：http://yzf.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://szs.zhixingplan.top

Go:   time.Now()
来源：http://pxl.andypj.xyz

Ruby: Time.now
来源：http://dgy.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tbk.sysykeji.top

[J02] 格式化输出
来源：http://dwu.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mwb.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ahx.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rdm.jiagoushi.top

TS:   d.toISOString()
来源：http://xuw.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vnd.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hbs.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hvh.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://veq.yfazqb.com

[J03] 字符串解析为日期
来源：http://nkx.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ypr.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gju.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://gtt.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://kuz.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gnz.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zwk.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://swl.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://seo.ydzc1.top

[J04] 时间戳与日期互转
来源：http://nul.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://scl.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oet.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pkq.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gyp.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qrn.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kyn.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vus.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mae.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://jcg.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://whv.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vba.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhs.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dbo.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://uyh.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rva.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://wxp.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://kdd.hnxiangtu.top

[J06] 计算两时间之差
来源：http://mze.aibaodan.cn


<!-- 参考信息 -->