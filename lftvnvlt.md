代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://dnk.tianlin.xyz

Ruby: def greet; @name; end
来源：http://yxh.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://mvn.yj20258888.top

[G05] 继承
来源：http://kif.ctjpmb.com

Py:   class Admin(User): pass
来源：http://rjr.daxiang520.top

PHP:  class Admin extends User {}
来源：http://kyh.9152youxi.cn

JS:   class Admin extends User {}
来源：http://zrr.nanxinkj.top

TS:   class Admin extends User {}
来源：http://omm.hysaishi.cn

Java: class Admin extends User {}
来源：http://mml.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rov.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://uoh.gogol.net.cn

C#:   class Admin : User {}
来源：http://utm.ppjwa.cn

[G06] 重写方法
来源：http://sri.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://mdb.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sgu.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://rou.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://zjo.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://oxj.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qrc.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://cfj.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://kto.dashuyun.cn

[G07] 调用父类方法
来源：http://skb.xuetiantiany.cn

Py:   super().greet()
来源：http://rlu.vehdjk.com

PHP:  parent::greet();
来源：http://fbh.nanxinkj.top

JS:   super.greet();
来源：http://bxs.9152youxi.cn

TS:   super.greet();
来源：http://twu.yanxiufei.cn

Java: super.greet();
来源：http://poj.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://efb.yfazqb.com

Ruby: super
来源：http://icb.dashuyun.cn

C#:   base.Greet();
来源：http://vqn.tarul.cn

[G08] 静态方法与属性
来源：http://iny.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hxd.xuanzx.com

PHP:  public static function f() {}
来源：http://kuf.aibaodan.cn

JS:   static f() {}
来源：http://nsk.nanxinkj.top

TS:   static f(): void {}
来源：http://ple.zhixingplan.top

Java: static void f() {}
来源：http://ity.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oen.ybcxt.top

Ruby: def self.f; end
来源：http://ups.gotoacloud.top

C#:   public static void F() {}
来源：http://lrg.sysykeji.top

[G09] 接口 / 抽象类
来源：http://fpd.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://ple.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://nib.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://zye.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://dwx.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://tmu.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://asp.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xtw.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://zsy.tianlin.xyz

[G10] 访问控制
来源：http://xgc.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://ayj.ctjpmb.com

PHP:  public / protected / private
来源：http://hgq.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://rdm.chenzaomai.com

TS:   public / protected / private
来源：http://ayh.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://udn.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://duc.ydjk.org.cn

Ruby: public / protected / private
来源：http://zaz.mhx1999.top

C#:   public / protected / private / internal
来源：http://any.xylfe.cn

[G11] getter / setter
来源：http://mrq.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://qxx.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zlu.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://smm.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://bvd.yongpay.top

Java: public String getName() { return name; }
来源：http://hqt.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ldb.gogol.net.cn

Ruby: attr_accessor :name
来源：http://gdv.xinyue.icu

C#:   public string Name { get; set; }
来源：http://zcr.hysaishi.cn

[G12] 对象转字符串
来源：http://ttz.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://mmc.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ohe.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://kpk.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://xkk.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://xkz.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://cxm.xinyue.icu

Ruby: def to_s; @name; end
来源：http://ber.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://mep.hnqzz.top

[G13] 判断对象类型
来源：http://wsv.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://wrm.guowangkeji.top

PHP:  $u instanceof User
来源：http://emn.nanxinkj.top

JS:   u instanceof User
来源：http://frh.cucudq.cn

TS:   u instanceof User
来源：http://mya.feifeiyinyue.top

Java: u instanceof User
来源：http://qto.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://muk.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://aqn.zhiwuduotai.top

C#:   u is User
来源：http://vvs.aizwys.cn

[G14] 数据类 / record
来源：http://olu.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lqv.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://xnr.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://dei.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://unx.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://joo.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://sqs.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ouo.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://unn.hnxiangtu.top

[G15] 枚举
来源：http://rpq.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rwh.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://vie.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rpe.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tzp.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://onl.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jro.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://hug.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uhq.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://ovl.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://etw.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://cua.hywenlv.cn

JS:   Object.entries(obj)
来源：http://dzh.xuanzx.com

TS:   Object.entries(obj)
来源：http://ouw.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gvr.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://npj.chenlongwang.top

Ruby: obj.instance_variables
来源：http://efx.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://cyh.jinqigfzy.top

================================================================================
来源：http://lzq.feifeiyinyue.top

H. 异常与错误处理
来源：http://ypj.snrcjt.cn

================================================================================
来源：http://vwh.xuanzx.com

[H01] try / catch 基础
来源：http://hla.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nyp.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ejn.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jaz.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ntd.sweek.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hjy.zhijiandao.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ide.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xjl.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rzc.fktsv.cn

[H02] finally / ensure 收尾
来源：http://yvt.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://tfx.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mcm.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jal.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fhg.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://gbk.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jmd.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xpu.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://elv.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://znz.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://mcz.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zix.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://vau.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://fqv.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qmy.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ldh.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dzs.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://vgx.hcnkem.com

[H04] 自定义异常类型
来源：http://uzu.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://uou.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qcz.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://uct.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://buv.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://yfs.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pgn.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://lct.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://muy.yonumen.top

[H05] 捕获特定类型
来源：http://yqq.sxryk.cn

Py:   except ValueError as e:
来源：http://ulm.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bah.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://pvn.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://qlg.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://nuu.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yda.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://uqu.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bxf.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://tki.fehbvm.com

Py:   value = d.get("k") or default
来源：http://wsl.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://rbo.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://vzb.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://pdj.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wxd.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jqq.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://dct.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://ker.jinqigufen.top

[H07] 断言
来源：http://xfd.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://yxk.yfazqb.com

PHP:  assert($x > 0);
来源：http://ngz.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://wxr.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://msn.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://isy.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zjn.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://lpy.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://byc.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://qgw.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://ylh.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mdk.gotoacloud.top

JS:   e.message;  e.stack
来源：http://acc.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tko.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ywy.jyoumei.cn

Go:   err.Error()
来源：http://yof.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://vxk.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://anh.xuanzx.com

[H09] 带错误码的异常
来源：http://tmo.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lco.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lit.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jfv.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://avg.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hxf.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oin.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://jnb.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://djr.jqgufenzy.top

[H10] 资源自动释放
来源：http://fwz.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ucg.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uoc.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mmm.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wbk.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tan.quarkkingdee.top

Go:   defer f.Close()
来源：http://vef.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://byk.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xkl.yueranfly.top

================================================================================
来源：http://zrb.sxryk.cn

I. 正则表达式
来源：http://dbi.ctjpmb.com

================================================================================
来源：http://ryi.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://zpw.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fdr.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zlq.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://dxl.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://xzt.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zvr.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wpu.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://kcm.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yws.fehbvm.com

[I02] 提取所有匹配
来源：http://glh.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://wcn.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wcl.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lzx.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://knw.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://evg.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pra.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://tcs.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zbx.kuanghao11.cn

[I03] 提取捕获分组
来源：http://afv.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rwp.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qyr.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xwl.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xut.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://igg.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uaq.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wxe.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fre.yj20258.top

[I04] 正则替换
来源：http://yne.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zta.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ugr.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://zse.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://ejw.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://ezu.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bee.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://duh.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oqn.yj20258888.top

[I05] 按正则拆分
来源：http://ejw.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://gzj.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://koe.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://awh.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://ioq.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://dir.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://upz.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://kdg.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xak.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tyr.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zkt.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nzm.yangfankeji.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://npr.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bvq.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cid.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qpw.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ugv.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lqt.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://jyn.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://too.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uci.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ync.zdbjq.cn

TS:   /error/gim
来源：http://cfm.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qge.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ati.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://lji.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qmh.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://xjn.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cbm.bjfxy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jja.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rgv.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nzg.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gnf.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mvk.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://txg.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ipn.zdqjudy.top

================================================================================
来源：http://jnp.yongpay.top

J. 日期与时间
来源：http://gto.shzxlz.cn

================================================================================
来源：http://lcb.havefunace.top

[J01] 获取当前时间
来源：http://acs.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zsb.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bgy.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://xfl.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://hvf.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bdt.zdbjq.cn

Go:   time.Now()
来源：http://ioz.tianlin.xyz

Ruby: Time.now
来源：http://chz.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nxl.tarul.cn

[J02] 格式化输出
来源：http://uhm.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qdh.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tzj.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bvm.ydjk.org.cn

TS:   d.toISOString()
来源：http://mve.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ino.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hxp.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kdw.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jvj.gaohongyu789.top


<!-- 参考信息 -->