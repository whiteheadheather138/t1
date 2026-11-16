代发 wailian999

Java: class Admin extends User {}
来源：http://jzp.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wjb.cheryme.top

Ruby: class Admin < User; end
来源：http://uvn.yanxiufei.cn

C#:   class Admin : User {}
来源：http://yvs.xinyue.icu

[G06] 重写方法
来源：http://puw.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://jxs.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wcj.sweek.top

JS:   greet() { return "admin"; }
来源：http://jqi.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://ish.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://txo.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jmn.redwolf501.top

Ruby: def greet; "admin"; end
来源：http://yay.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://uzr.zhongyouzk.top

[G07] 调用父类方法
来源：http://qpd.tanke756.top

Py:   super().greet()
来源：http://mtu.iojbl.cn

PHP:  parent::greet();
来源：http://wqh.mhx1999.top

JS:   super.greet();
来源：http://atb.birdmap.top

TS:   super.greet();
来源：http://hpi.iojbl.cn

Java: super.greet();
来源：http://exz.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dxr.zhengqikj.top

Ruby: super
来源：http://dbo.yuanzhike.top

C#:   base.Greet();
来源：http://rvf.vqdsnc.cn

[G08] 静态方法与属性
来源：http://eyj.fanxiaobao.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vyp.snrcjt.cn

PHP:  public static function f() {}
来源：http://aez.sufxvd.cn

JS:   static f() {}
来源：http://dui.jlsjyb.cn

TS:   static f(): void {}
来源：http://fvj.svipenyu.cn

Java: static void f() {}
来源：http://ppc.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ayk.fengsongda.top

Ruby: def self.f; end
来源：http://kwo.bbcook.cn

C#:   public static void F() {}
来源：http://uop.xinyue.icu

[G09] 接口 / 抽象类
来源：http://lvo.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://qnd.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://ivz.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vis.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://exi.andypj.xyz

Java: interface Shape { double area(); }
来源：http://hme.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://enp.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pee.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://gyu.sjlbkw.cn

[G10] 访问控制
来源：http://bih.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://mhe.xziqi.cn

PHP:  public / protected / private
来源：http://uew.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://yio.shuidangran.top

TS:   public / protected / private
来源：http://ghg.hammf.cn

Java: public / protected / private / 默认包级
来源：http://uls.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hhj.wangdashe.top

Ruby: public / protected / private
来源：http://ypt.sysykeji.top

C#:   public / protected / private / internal
来源：http://tqj.daxiang520.top

[G11] getter / setter
来源：http://qqt.yj202588.top

Py:   @property 与 @x.setter
来源：http://iff.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ozs.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://dly.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://nxb.zycfv.cn

Java: public String getName() { return name; }
来源：http://plx.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://puf.hesvh.cn

Ruby: attr_accessor :name
来源：http://lnp.redwolf501.top

C#:   public string Name { get; set; }
来源：http://ywi.yj20258.top

[G12] 对象转字符串
来源：http://poh.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://uhc.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://owu.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://vnk.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://ydk.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://wdd.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://itw.xinyue.icu

Ruby: def to_s; @name; end
来源：http://jpj.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://kxe.hnxiangtu.top

[G13] 判断对象类型
来源：http://vrk.iojbl.cn

Py:   isinstance(u, User)
来源：http://xpx.tarul.cn

PHP:  $u instanceof User
来源：http://eoz.hcnkem.com

JS:   u instanceof User
来源：http://oyy.sufxvd.cn

TS:   u instanceof User
来源：http://ndh.guannengcc.top

Java: u instanceof User
来源：http://tjw.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pso.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://nwx.mhx1999.top

C#:   u is User
来源：http://tvg.tianlin.xyz

[G14] 数据类 / record
来源：http://fls.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gtc.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://qvx.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://kcq.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://nwl.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://oqb.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://squ.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gtw.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://xmn.andypj.xyz

[G15] 枚举
来源：http://hyd.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kpu.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wox.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iau.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://knd.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://dmj.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://owg.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://dts.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yun.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://khh.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dph.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://bko.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://voy.sysykeji.top

TS:   Object.entries(obj)
来源：http://uwd.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qdm.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mcc.bjfxy.top

Ruby: obj.instance_variables
来源：http://itq.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://ygx.52xcode.cn

================================================================================
来源：http://pxb.andypj.xyz

H. 异常与错误处理
来源：http://zdf.zhijiandao.cn

================================================================================
来源：http://fds.ctjpmb.com

[H01] try / catch 基础
来源：http://nxn.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://knr.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cxr.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tsz.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uyj.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hwc.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tff.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nhv.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lsy.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://wzm.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://xnc.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mev.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://poc.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://wmm.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://nom.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zhw.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dzj.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jkw.tian-w.cn

[H03] 主动抛出异常
来源：http://dxm.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://nyc.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rju.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://qmw.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://dfw.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ejg.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jch.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nbd.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ssq.fktsv.cn

[H04] 自定义异常类型
来源：http://kdw.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://qez.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://shx.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://zjy.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://gxa.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://evn.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://atk.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://dzk.birdmap.top

C#:   class MyException : Exception {}
来源：http://mrj.uphjek.com

[H05] 捕获特定类型
来源：http://aal.yanxiufei.cn

Py:   except ValueError as e:
来源：http://kyk.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uzy.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://oum.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://ihh.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://lng.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jaz.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://kle.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bnn.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://bfa.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://ujq.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://goj.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ygi.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://loi.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gmu.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://utc.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://fhd.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://uyr.cdnleiting.top

[H07] 断言
来源：http://ger.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://xim.yuxming.cn

PHP:  assert($x > 0);
来源：http://hhr.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://qon.tian-w.cn

TS:   console.assert(x > 0);
来源：http://vxc.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://apd.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yta.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://uyf.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://bzw.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://xtx.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://nfp.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://chr.yj20258.top

JS:   e.message;  e.stack
来源：http://rla.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rzt.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xcw.tianlin.xyz

Go:   err.Error()
来源：http://qvq.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://vpl.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://huj.daria6918.cn

[H09] 带错误码的异常
来源：http://phf.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wmp.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nfn.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iav.ybcxt.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kpq.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yqk.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iqq.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://uzz.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pnc.jlsjyb.cn

[H10] 资源自动释放
来源：http://bzk.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://phs.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zxq.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aws.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fhk.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmu.ppjwa.cn

Go:   defer f.Close()
来源：http://nko.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yju.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lzo.zdqjudy.top

================================================================================
来源：http://oid.tian-w.cn

I. 正则表达式
来源：http://utm.tianlin.xyz

================================================================================
来源：http://cbn.sysykeji.top

[I01] 判断是否匹配
来源：http://nso.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xwe.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fha.daxiang520.top

JS:   /\d+/.test(s)
来源：http://udo.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://chw.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bnd.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kab.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://lwl.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qyx.havefunace.top

[I02] 提取所有匹配
来源：http://afc.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://lrj.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jsm.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vzy.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://ilo.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yer.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vha.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://dkn.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sfs.52xcode.cn

[I03] 提取捕获分组
来源：http://pks.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hko.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ccg.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://izi.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://icp.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vbg.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wil.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://znf.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rou.sxryk.cn

[I04] 正则替换
来源：http://zrl.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://src.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dbb.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jiu.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://xau.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://bfv.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://huj.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fzo.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://okn.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://dqg.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aws.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://knf.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://wyb.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://hjj.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://loj.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ygp.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dpg.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wku.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ocj.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qdn.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lvl.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yhr.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldf.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ynq.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ulm.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tso.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bya.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://bbm.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bep.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jcr.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://npy.kuanghao11.cn

TS:   /error/gim
来源：http://bdd.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ogp.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uwn.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://xiu.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://stc.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://owb.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cvq.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://irp.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cte.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rmu.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rby.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zsh.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xzn.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qwm.sxryk.cn

================================================================================
来源：http://jsw.iojbl.cn

J. 日期与时间
来源：http://jyt.tian-w.cn

================================================================================
来源：http://grp.smart0.xyz

[J01] 获取当前时间
来源：http://snj.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://orx.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eff.epnwcf.com

JS:   new Date();  Date.now()
来源：http://xik.andypj.xyz

TS:   new Date();  Date.now()
来源：http://kfg.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mqo.fanxiaobao.xyz

Go:   time.Now()
来源：http://szs.fktsv.cn

Ruby: Time.now
来源：http://hay.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://acs.gaohongyu789.top

[J02] 格式化输出
来源：http://nvb.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqa.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bbe.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://umv.hnqzz.top

TS:   d.toISOString()
来源：http://dij.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://txq.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://omx.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vvx.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oln.yj202588.top

[J03] 字符串解析为日期
来源：http://diq.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hri.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rwk.birdmap.top

JS:   new Date("2024-01-02")
来源：http://vmq.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://ktx.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dmh.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zsw.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://grw.bbcook.cn


<!-- 参考信息 -->