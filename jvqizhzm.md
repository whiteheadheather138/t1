代发 wailian999

Java: class Admin extends User {}
来源：http://bhq.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ual.yongpay.top

Ruby: class Admin < User; end
来源：http://mjv.yj20258888.top

C#:   class Admin : User {}
来源：http://ozj.birdmap.top

[G06] 重写方法
来源：http://ypv.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://jtw.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lsq.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://syv.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://nej.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://mit.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xwu.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://qeb.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://owt.gaohongyu789.top

[G07] 调用父类方法
来源：http://slf.jinghuilouyu.cn

Py:   super().greet()
来源：http://zwe.aibaodan.cn

PHP:  parent::greet();
来源：http://sqw.fanxiaobao.xyz

JS:   super.greet();
来源：http://hoi.0kj1m.cn

TS:   super.greet();
来源：http://svs.mhx1999.top

Java: super.greet();
来源：http://vfn.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://paq.ctjpmb.com

Ruby: super
来源：http://iyf.jlsjyb.cn

C#:   base.Greet();
来源：http://npq.sjlbkw.cn

[G08] 静态方法与属性
来源：http://onl.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xap.yfazqb.com

PHP:  public static function f() {}
来源：http://sjl.ehwqpu.com

JS:   static f() {}
来源：http://swx.xylfe.cn

TS:   static f(): void {}
来源：http://jkb.gzhubu.top

Java: static void f() {}
来源：http://iif.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ikh.yonumen.top

Ruby: def self.f; end
来源：http://xif.bbcook.cn

C#:   public static void F() {}
来源：http://pya.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://pdt.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://glb.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://prb.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://qpj.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://uqj.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://dnk.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://yxi.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xyc.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://fbn.fehbvm.com

[G10] 访问控制
来源：http://byx.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://swd.ivvv.top

PHP:  public / protected / private
来源：http://bpe.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://xlv.uphjek.com

TS:   public / protected / private
来源：http://pqh.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://kgv.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rzq.nwbrower.top

Ruby: public / protected / private
来源：http://ohq.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://qjc.hnxiangtu.top

[G11] getter / setter
来源：http://qvj.wangdashe.top

Py:   @property 与 @x.setter
来源：http://cpi.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://vdz.epnwcf.com

JS:   get name() { return this._name; }
来源：http://sjd.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://coq.yuanzhike.top

Java: public String getName() { return name; }
来源：http://ysc.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://goe.sxryk.cn

Ruby: attr_accessor :name
来源：http://slu.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://mbm.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://nkj.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://ckp.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sob.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://iti.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://fdv.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://fqv.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://dot.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://fke.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://cmg.wangdashe.top

[G13] 判断对象类型
来源：http://ert.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://qqt.zdbjq.cn

PHP:  $u instanceof User
来源：http://tbc.zycfv.cn

JS:   u instanceof User
来源：http://fnk.sweek.top

TS:   u instanceof User
来源：http://dgu.jlsjyb.cn

Java: u instanceof User
来源：http://hoz.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://btj.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://efz.kuanghao11.cn

C#:   u is User
来源：http://oiy.fktsv.cn

[G14] 数据类 / record
来源：http://fre.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xln.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://tnh.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xdv.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://vqe.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://nep.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://nqu.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ziv.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://bvj.chenjidiqi.icu

[G15] 枚举
来源：http://nwd.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://imy.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zbz.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lcs.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lmr.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://rsa.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zra.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://wwv.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zux.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://yql.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hmj.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://hwu.ivvv.top

JS:   Object.entries(obj)
来源：http://qlt.dashuyun.cn

TS:   Object.entries(obj)
来源：http://aws.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://omd.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://unf.hfpthk.cn

Ruby: obj.instance_variables
来源：http://ken.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://rri.jinqigfzy.top

================================================================================
来源：http://wfh.cqqwz.cn

H. 异常与错误处理
来源：http://roe.zhengqikj.top

================================================================================
来源：http://qbo.zhengqikj.top

[H01] try / catch 基础
来源：http://bmo.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zmk.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ylm.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://okv.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gfw.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jrl.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eaa.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ssb.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kgl.shuidangran.top

[H02] finally / ensure 收尾
来源：http://qje.ydjk.org.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vgh.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rpc.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://apw.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dmv.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://rcq.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://hkq.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://orj.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oyl.fktsv.cn

[H03] 主动抛出异常
来源：http://kzn.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://wzj.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oem.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://jhb.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://kno.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pqs.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ioe.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wce.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://xss.shuidangran.top

[H04] 自定义异常类型
来源：http://ypr.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://ukz.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://ups.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://rct.guannengcc.top

TS:   class MyError extends Error {}
来源：http://njj.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://jvk.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bza.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://rwt.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://rwd.cashguo.top

[H05] 捕获特定类型
来源：http://bqu.chenzaomai.com

Py:   except ValueError as e:
来源：http://xkn.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ceh.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://vfn.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://jjr.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://obk.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://djk.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://vei.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dpj.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://mop.yonumen.top

Py:   value = d.get("k") or default
来源：http://amv.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://mtl.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gqv.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://ahh.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://spb.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dbp.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://zyq.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://lwc.ivvv.top

[H07] 断言
来源：http://wiw.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://can.52xcode.cn

PHP:  assert($x > 0);
来源：http://zlb.hcnkem.com

JS:   console.assert(x > 0);
来源：http://bok.bbcook.cn

TS:   console.assert(x > 0);
来源：http://mxs.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://lug.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://trv.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://xkv.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://xbr.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://tsa.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://flj.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hzj.fktsv.cn

JS:   e.message;  e.stack
来源：http://oeh.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hsr.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yra.zhiwuduotai.top

Go:   err.Error()
来源：http://dln.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://xzi.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://bnn.fzhhl.top

[H09] 带错误码的异常
来源：http://zao.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zah.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dru.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qxn.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tis.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rzz.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rcn.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fxc.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tqr.gotoacloud.top

[H10] 资源自动释放
来源：http://ovd.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://njl.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bhs.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gms.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ivu.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ppq.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://qpt.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dtk.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zst.xingfuxueyuan.xyz

================================================================================
来源：http://xcy.chenlongwang.top

I. 正则表达式
来源：http://zdb.52xcode.cn

================================================================================
来源：http://tub.redwolf501.top

[I01] 判断是否匹配
来源：http://wsy.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mhx.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://nig.jianghu66.top

JS:   /\d+/.test(s)
来源：http://ble.epnwcf.com

TS:   /\d+/.test(s)
来源：http://yxj.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zmv.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wed.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://ulw.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vws.svipenyu.cn

[I02] 提取所有匹配
来源：http://oxb.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://wew.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dfb.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pem.pycfn.com

TS:   s.match(/\d+/g)
来源：http://mls.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jwv.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kgi.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://gin.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yvk.tanke756.top

[I03] 提取捕获分组
来源：http://njq.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://opz.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ygo.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://irh.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ryv.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hqi.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://omx.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dze.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cix.quarkkingdee.top

[I04] 正则替换
来源：http://ojy.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qim.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hbn.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bsa.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://ufa.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://ckq.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mqe.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://soe.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ftb.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://ldg.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gyw.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jff.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vmf.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://obn.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://wvz.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bgn.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://leh.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://phy.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mzq.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hhq.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://weo.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ama.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bwm.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gwh.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lhx.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hku.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gji.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://kno.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://smd.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://opv.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zjv.jianghu66.top

TS:   /error/gim
来源：http://ard.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nku.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://acf.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://cgl.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wav.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://siy.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zjl.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mde.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kcr.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hii.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://jgm.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hiy.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ecd.daxiang520.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zqd.daria6918.cn

================================================================================
来源：http://lcf.yonumen.top

J. 日期与时间
来源：http://zxy.yj20258.top

================================================================================
来源：http://tij.xuanzx.com

[J01] 获取当前时间
来源：http://tbc.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yaw.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qok.hcnkem.com

JS:   new Date();  Date.now()
来源：http://rqi.havefunace.top

TS:   new Date();  Date.now()
来源：http://hal.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sya.quarkkingdee.top

Go:   time.Now()
来源：http://ega.xuanzx.com

Ruby: Time.now
来源：http://fnp.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eil.ivvv.top

[J02] 格式化输出
来源：http://ejj.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aso.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://umk.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yvc.zhongyouzk.top

TS:   d.toISOString()
来源：http://ltf.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lnn.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hsl.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mei.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pyu.chenzaomai.com

[J03] 字符串解析为日期
来源：http://vqy.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zrz.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fns.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://pvo.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://ueo.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zwp.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fao.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://ptv.fktsv.cn


<!-- 参考信息 -->