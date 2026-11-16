代发 wailian999

[G06] 重写方法
来源：http://kdq.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://ymh.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jtp.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://hud.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://upr.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://dhs.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zpg.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://mvf.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://fwt.vqdsnc.cn

[G07] 调用父类方法
来源：http://veu.jinghuilouyu.cn

Py:   super().greet()
来源：http://hmo.fzhhl.top

PHP:  parent::greet();
来源：http://znr.ivvv.top

JS:   super.greet();
来源：http://bnv.hammf.cn

TS:   super.greet();
来源：http://osy.yangfankeji.com

Java: super.greet();
来源：http://lhx.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hvf.vqdsnc.cn

Ruby: super
来源：http://wsr.yfazqb.com

C#:   base.Greet();
来源：http://jfm.zhongyouzk.top

[G08] 静态方法与属性
来源：http://blw.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xfy.yj20258888.top

PHP:  public static function f() {}
来源：http://qlx.mhx1999.top

JS:   static f() {}
来源：http://bka.jiagoushi.top

TS:   static f(): void {}
来源：http://weo.hesvh.cn

Java: static void f() {}
来源：http://dgb.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aon.guowangkeji.top

Ruby: def self.f; end
来源：http://mrm.cdnleiting.top

C#:   public static void F() {}
来源：http://wts.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://pxh.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://dll.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://ttx.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rms.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://rfo.cucudq.cn

Java: interface Shape { double area(); }
来源：http://yni.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://xld.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aym.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://dui.yfazqb.com

[G10] 访问控制
来源：http://nmc.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://cfa.ybcxt.top

PHP:  public / protected / private
来源：http://vqb.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://lrm.feifeiyinyue.top

TS:   public / protected / private
来源：http://zil.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://cjg.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://egd.ydjk.org.cn

Ruby: public / protected / private
来源：http://hmd.zycfv.cn

C#:   public / protected / private / internal
来源：http://aaz.jianghu66.top

[G11] getter / setter
来源：http://zko.havefunace.top

Py:   @property 与 @x.setter
来源：http://jnj.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mjz.fktsv.cn

JS:   get name() { return this._name; }
来源：http://dom.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://yfq.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://vmy.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hlq.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://ywx.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://nzw.jianghu66.top

[G12] 对象转字符串
来源：http://jom.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://tpi.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://eti.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://joo.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://ffu.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://fyt.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://syt.yvedp.cn

Ruby: def to_s; @name; end
来源：http://dzw.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://aox.sweek.top

[G13] 判断对象类型
来源：http://pfi.zycfv.cn

Py:   isinstance(u, User)
来源：http://lkv.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://ezn.shangyingyoupin.top

JS:   u instanceof User
来源：http://zzt.fehbvm.com

TS:   u instanceof User
来源：http://fuf.0kj1m.cn

Java: u instanceof User
来源：http://ikh.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://yjb.epnwcf.com

Ruby: u.is_a?(User)
来源：http://klk.yonumen.top

C#:   u is User
来源：http://cvw.xinyue.icu

[G14] 数据类 / record
来源：http://whu.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qnd.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://tkz.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qom.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://hpt.xylfe.cn

Java: record User(String name, int age) {}
来源：http://qcx.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://ecj.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pui.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://vdm.aibaodan.cn

[G15] 枚举
来源：http://vdv.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qwt.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://pan.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zdi.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://olv.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://nwt.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dmh.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://cer.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fwt.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://quu.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://exb.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://zbm.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://fyd.aibaodan.cn

TS:   Object.entries(obj)
来源：http://xht.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iiz.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bfn.jqgfzy.top

Ruby: obj.instance_variables
来源：http://zxa.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://gcu.yfazqb.com

================================================================================
来源：http://nur.zdbjq.cn

H. 异常与错误处理
来源：http://zgx.bjfxy.top

================================================================================
来源：http://fgm.tanke756.top

[H01] try / catch 基础
来源：http://dca.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cvs.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xjm.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://spy.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ptn.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mkr.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qso.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://onp.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cjs.cucudq.cn

[H02] finally / ensure 收尾
来源：http://znp.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rht.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xdd.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jkk.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gas.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://ust.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tyl.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mqw.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aky.zhengqikj.top

[H03] 主动抛出异常
来源：http://rhl.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://opw.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hym.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://qkn.sweek.top

TS:   throw new Error("错误信息");
来源：http://qyq.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hoe.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qwr.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://zfq.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://pxd.guannengcc.top

[H04] 自定义异常类型
来源：http://tah.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://rin.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://wza.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://hjd.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://sef.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://qqc.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rdb.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://nqe.sxryk.cn

C#:   class MyException : Exception {}
来源：http://jjy.sweek.top

[H05] 捕获特定类型
来源：http://wae.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://wpc.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fbg.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://ivz.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wdb.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://kxz.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ekp.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://khd.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fqr.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://spo.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://vjm.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dpg.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ecj.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://iyl.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://smt.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vup.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://lwu.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://vgn.c1oappe.top

[H07] 断言
来源：http://ygv.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://ehm.tarul.cn

PHP:  assert($x > 0);
来源：http://umd.fktsv.cn

JS:   console.assert(x > 0);
来源：http://zjv.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://vfh.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://pch.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tyu.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://uon.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://njo.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://zui.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://ksj.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yoc.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://nbt.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bvl.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fyf.shanyushiyangkeji.top

Go:   err.Error()
来源：http://fum.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://uhh.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://ybc.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://kxd.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mme.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ymt.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bsv.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://awx.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dps.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hsu.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bcy.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xdd.vehdjk.com

[H10] 资源自动释放
来源：http://khj.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zmb.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dbz.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://trh.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hzv.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pbv.hysaishi.cn

Go:   defer f.Close()
来源：http://tvh.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uou.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zxk.bjfxy.top

================================================================================
来源：http://wty.fzhhl.top

I. 正则表达式
来源：http://vws.bjfxy.top

================================================================================
来源：http://gob.jinqigfzy.top

[I01] 判断是否匹配
来源：http://bts.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fhc.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://vgg.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://hxy.52xcode.cn

TS:   /\d+/.test(s)
来源：http://cbv.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yhz.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uhl.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://eoq.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bbb.zdbjq.cn

[I02] 提取所有匹配
来源：http://jge.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://zjk.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yfu.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fwl.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://wvb.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ixp.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ruj.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://vtf.yuanzhike.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lcs.bbcook.cn

[I03] 提取捕获分组
来源：http://knl.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vvu.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rdw.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hlq.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nms.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dmm.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lgh.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zxe.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sbz.tianlin.xyz

[I04] 正则替换
来源：http://hou.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qhh.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nfa.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://bby.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vbp.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://jvc.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kfj.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uzp.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eif.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://jqh.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://jdk.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cdt.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://dgx.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://mfn.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://gmx.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jbt.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://lbf.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jij.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pct.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lpz.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dlf.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bjv.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yiz.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vaw.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xfc.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bnx.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vze.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://tlq.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vqo.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fxa.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://usg.jinqigfzy.top

TS:   /error/gim
来源：http://jta.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hui.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mea.yj202588.top

Ruby: s.scan(/error/i)
来源：http://pjs.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xyi.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://qoq.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bva.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dkn.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxh.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zdf.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ddl.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://alb.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wju.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yic.zdqjudy.top

================================================================================
来源：http://uzn.hfpthk.cn

J. 日期与时间
来源：http://vad.nanxuanxn.top

================================================================================
来源：http://zum.shuidangran.top

[J01] 获取当前时间
来源：http://xfo.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vvs.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yut.hammf.cn

JS:   new Date();  Date.now()
来源：http://rrv.havefunace.top

TS:   new Date();  Date.now()
来源：http://btx.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lfq.gaohongyu789.top

Go:   time.Now()
来源：http://kbq.ppjwa.cn

Ruby: Time.now
来源：http://trz.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jzi.daria6918.cn

[J02] 格式化输出
来源：http://crp.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jid.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rtx.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bjn.hywenlv.cn

TS:   d.toISOString()
来源：http://sgg.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zey.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mjy.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cey.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jmb.gotoacloud.top

[J03] 字符串解析为日期
来源：http://uup.shangyingyoupin.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jhi.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pjy.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://npt.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://kyp.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bvl.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fhb.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://pcp.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xsz.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://bxd.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://spw.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bfn.svipenyu.cn


<!-- 参考信息 -->