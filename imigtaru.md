代发 wailian999

Java: class Admin extends User {}
来源：http://iuj.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xgk.vehdjk.com

Ruby: class Admin < User; end
来源：http://hjv.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://wqy.yfazqb.com

[G06] 重写方法
来源：http://rqw.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://owh.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vjp.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://uji.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://nsy.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://owz.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sye.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://rjc.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://ney.birdmap.top

[G07] 调用父类方法
来源：http://gam.hnxiangtu.top

Py:   super().greet()
来源：http://ihr.shzxlz.cn

PHP:  parent::greet();
来源：http://xbk.zhaomingkeji.xyz

JS:   super.greet();
来源：http://cst.aibaodan.cn

TS:   super.greet();
来源：http://axm.guannengcc.top

Java: super.greet();
来源：http://ltm.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://res.dashuyun.cn

Ruby: super
来源：http://rvn.9152youxi.cn

C#:   base.Greet();
来源：http://edc.yangfankeji.com

[G08] 静态方法与属性
来源：http://wrs.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://msp.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://vdh.quarkkingdee.top

JS:   static f() {}
来源：http://jdj.uphjek.com

TS:   static f(): void {}
来源：http://nws.wangshuangyany.cn

Java: static void f() {}
来源：http://bxj.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zgt.cashguo.top

Ruby: def self.f; end
来源：http://zsk.nanxuanxn.top

C#:   public static void F() {}
来源：http://yhi.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://hat.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://bph.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qyl.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kph.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://mps.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://wjg.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://jtb.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zjt.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://zwl.yanxiufei.cn

[G10] 访问控制
来源：http://coe.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://qmi.gzhubu.top

PHP:  public / protected / private
来源：http://msh.fehbvm.com

JS:   #private 字段；其余公开
来源：http://pfb.jyoumei.cn

TS:   public / protected / private
来源：http://fwo.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://wpv.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://jhy.gaohongyu789.top

Ruby: public / protected / private
来源：http://snn.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://tdf.cqqwz.cn

[G11] getter / setter
来源：http://sxp.fktsv.cn

Py:   @property 与 @x.setter
来源：http://gii.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rah.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://wzk.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://jde.sxryk.cn

Java: public String getName() { return name; }
来源：http://sgx.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jma.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://fav.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://mur.yj202588.top

[G12] 对象转字符串
来源：http://qtf.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://muq.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xoi.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://ewl.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://vbm.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://njo.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://bbc.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://lfq.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://dzi.tianlin.xyz

[G13] 判断对象类型
来源：http://dhu.ivvv.top

Py:   isinstance(u, User)
来源：http://omb.fengsongda.top

PHP:  $u instanceof User
来源：http://ahy.yvedp.cn

JS:   u instanceof User
来源：http://quj.shzxlz.cn

TS:   u instanceof User
来源：http://efu.cheryme.top

Java: u instanceof User
来源：http://vtq.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sre.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://cej.dianchejie.cn

C#:   u is User
来源：http://ivt.gogol.net.cn

[G14] 数据类 / record
来源：http://jkp.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kax.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://hiv.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://trt.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://ces.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://uzw.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://mlj.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hrs.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://fer.pengpengdd.cyou

[G15] 枚举
来源：http://gba.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ebu.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://btt.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mdr.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lgb.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://lbt.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zrr.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://huu.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bwi.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://gio.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lld.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://kzt.mhx1999.top

JS:   Object.entries(obj)
来源：http://vue.zhengqikj.top

TS:   Object.entries(obj)
来源：http://rya.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kia.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yge.andypj.xyz

Ruby: obj.instance_variables
来源：http://xtx.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://lxr.zhoulong.xyz

================================================================================
来源：http://qbs.316326.xyz

H. 异常与错误处理
来源：http://vrd.tianlin.xyz

================================================================================
来源：http://kkb.ppjwa.cn

[H01] try / catch 基础
来源：http://jjk.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ixi.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qfd.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mtj.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xme.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wum.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dua.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eam.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xey.jianghu66.top

[H02] finally / ensure 收尾
来源：http://hdb.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://mrh.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hbl.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pav.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qac.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://qcs.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://ghf.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://nws.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sum.dianchejie.cn

[H03] 主动抛出异常
来源：http://qxh.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://rjq.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dvg.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://rqa.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://ncd.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qwk.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dhm.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oor.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://jdr.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://ptt.yj202588.top

Py:   class MyError(Exception): pass
来源：http://lvk.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://cyr.yuxming.cn

JS:   class MyError extends Error {}
来源：http://kht.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://fhz.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://gmp.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lli.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://ejq.hysaishi.cn

C#:   class MyException : Exception {}
来源：http://jev.sufxvd.cn

[H05] 捕获特定类型
来源：http://sro.0kj1m.cn

Py:   except ValueError as e:
来源：http://rio.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sso.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://hqt.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://vcc.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://ziw.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ypg.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://fjt.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mcz.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://qog.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://dxh.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wjz.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://tpx.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://chb.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dfm.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hcz.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://fix.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://pge.nanxuanxn.top

[H07] 断言
来源：http://uuj.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://bds.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://wsw.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://tai.hesvh.cn

TS:   console.assert(x > 0);
来源：http://mal.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://jjc.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ozl.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vby.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://dvr.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://obv.kuanghao11.cn

Py:   str(e);  traceback.format_exc()
来源：http://zpw.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lzh.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://mri.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vwr.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xpi.hysaishi.cn

Go:   err.Error()
来源：http://wcp.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://igo.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://dah.tian-w.cn

[H09] 带错误码的异常
来源：http://gxb.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hia.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://eiw.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tyc.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cyi.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mlb.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zux.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://lhq.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://mvj.316326.xyz

[H10] 资源自动释放
来源：http://ttb.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yjr.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gds.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qlr.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jfq.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://unt.xuetiantiany.cn

Go:   defer f.Close()
来源：http://xxu.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dsh.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dst.dianchejie.cn

================================================================================
来源：http://zsu.fktsv.cn

I. 正则表达式
来源：http://hll.ydzc1.top

================================================================================
来源：http://lsn.nanxuanxn.top

[I01] 判断是否匹配
来源：http://wgx.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dpu.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://led.jianghu66.top

JS:   /\d+/.test(s)
来源：http://dmh.yongpay.top

TS:   /\d+/.test(s)
来源：http://byx.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hbk.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ily.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://ugb.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qzr.birdmap.top

[I02] 提取所有匹配
来源：http://ahy.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://ukx.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vda.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://egh.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://hsg.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://czz.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://knh.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://heh.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bxm.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://roe.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cxu.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jgh.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mos.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pex.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hbg.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bcs.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bhu.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wrc.jqgfzy.top

[I04] 正则替换
来源：http://oaj.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fou.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pfz.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://ruf.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://syb.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ucf.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://kxo.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://dee.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://der.cheryme.top

[I05] 按正则拆分
来源：http://wzf.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mey.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://alj.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://bqy.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://npx.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://tqj.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wms.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://ays.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nfk.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yjk.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rfn.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zcz.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vfw.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pkl.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wbi.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eyx.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bsz.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://roq.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://icc.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wzh.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dfr.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tsu.daxiang520.top

TS:   /error/gim
来源：http://fdr.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rho.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sqq.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://ifa.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xyk.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://obm.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lyh.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cmj.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgu.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nql.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://slm.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hpd.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ypn.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wjk.epnwcf.com

================================================================================
来源：http://afk.bjfxy.top

J. 日期与时间
来源：http://wzy.gotoacloud.top

================================================================================
来源：http://vtu.guowangkeji.top

[J01] 获取当前时间
来源：http://nzz.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qix.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://def.xylfe.cn

JS:   new Date();  Date.now()
来源：http://qum.yfazqb.com

TS:   new Date();  Date.now()
来源：http://bil.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://wnp.c1oappe.top

Go:   time.Now()
来源：http://yxl.yueranfly.top

Ruby: Time.now
来源：http://mqv.hnxiangtu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gpp.aibaodan.cn

[J02] 格式化输出
来源：http://nmi.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://szn.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://opw.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jld.hnxiangtu.top

TS:   d.toISOString()
来源：http://uhu.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zmn.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lzu.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lbj.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ihr.havefunace.top

[J03] 字符串解析为日期
来源：http://zub.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xci.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://avx.316326.xyz

JS:   new Date("2024-01-02")
来源：http://bad.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://jqb.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://jhe.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gev.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://jjq.smart0.xyz


<!-- 参考信息 -->