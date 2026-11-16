代发 wailian999

Ruby: @name = "x"
来源：http://lgj.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://unb.yuxming.cn

[G04] 定义方法
来源：http://ehy.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://ryy.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://apg.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://jib.cashguo.top

TS:   greet(): string { return this.name; }
来源：http://anl.sjlbkw.cn

Java: String greet() { return name; }
来源：http://asm.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://idw.sxryk.cn

Ruby: def greet; @name; end
来源：http://yhx.shuidangran.top

C#:   public string Greet() => Name;
来源：http://gki.cheryme.top

[G05] 继承
来源：http://lch.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://nee.xziqi.cn

PHP:  class Admin extends User {}
来源：http://nqd.wangdashe.top

JS:   class Admin extends User {}
来源：http://qvv.ppjwa.cn

TS:   class Admin extends User {}
来源：http://ica.xinyue.icu

Java: class Admin extends User {}
来源：http://myb.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rwr.yueranfly.top

Ruby: class Admin < User; end
来源：http://soy.yfazqb.com

C#:   class Admin : User {}
来源：http://scd.aizwys.cn

[G06] 重写方法
来源：http://sgl.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://yre.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mok.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://sxl.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://vki.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://jlw.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gfi.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://gvf.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://lvc.tanke756.top

[G07] 调用父类方法
来源：http://ejj.jianghu66.top

Py:   super().greet()
来源：http://iyg.cqqwz.cn

PHP:  parent::greet();
来源：http://djs.yonumen.top

JS:   super.greet();
来源：http://ezk.hnqzz.top

TS:   super.greet();
来源：http://mrn.vqdsnc.cn

Java: super.greet();
来源：http://xim.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ejl.ydzc1.top

Ruby: super
来源：http://qnr.zhoulong.xyz

C#:   base.Greet();
来源：http://ttc.hywenlv.cn

[G08] 静态方法与属性
来源：http://zjr.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kau.hysaishi.cn

PHP:  public static function f() {}
来源：http://oxb.xinyue.icu

JS:   static f() {}
来源：http://gkn.daxiang520.top

TS:   static f(): void {}
来源：http://kva.uphjek.com

Java: static void f() {}
来源：http://cmd.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://qdw.xuetiantiany.cn

Ruby: def self.f; end
来源：http://got.dashuyun.cn

C#:   public static void F() {}
来源：http://fkn.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://oei.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://che.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xfv.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://evg.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://gjv.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://lsu.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://gad.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yke.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://olx.aibaodan.cn

[G10] 访问控制
来源：http://wrn.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://xno.zycfv.cn

PHP:  public / protected / private
来源：http://vkk.vehdjk.com

JS:   #private 字段；其余公开
来源：http://gxx.yanxiufei.cn

TS:   public / protected / private
来源：http://tll.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://xjj.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bad.xinyue.icu

Ruby: public / protected / private
来源：http://gtb.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://mrs.chenjidiqi.icu

[G11] getter / setter
来源：http://kyq.xylfe.cn

Py:   @property 与 @x.setter
来源：http://uqp.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cwu.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://rwk.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://fyl.nanxinkj.top

Java: public String getName() { return name; }
来源：http://pwj.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://evp.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://kqg.mhx1999.top

C#:   public string Name { get; set; }
来源：http://ucy.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://stn.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://tda.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wlo.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://uvm.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://yqt.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://ycq.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://ztw.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://gho.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://uzi.xinyue.icu

[G13] 判断对象类型
来源：http://wip.316326.xyz

Py:   isinstance(u, User)
来源：http://zli.dashuyun.cn

PHP:  $u instanceof User
来源：http://pyu.tanke756.top

JS:   u instanceof User
来源：http://efw.feifeiyinyue.top

TS:   u instanceof User
来源：http://flb.shangyingyoupin.top

Java: u instanceof User
来源：http://kea.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mzb.yj20258888.top

Ruby: u.is_a?(User)
来源：http://zzc.yj202588.top

C#:   u is User
来源：http://hej.sweek.top

[G14] 数据类 / record
来源：http://yhk.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uqk.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://mot.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://dag.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://zti.ydzc1.top

Java: record User(String name, int age) {}
来源：http://qjb.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://pjf.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://btk.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://xgf.cheryme.top

[G15] 枚举
来源：http://soq.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xfg.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsg.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iyl.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qhl.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://vnw.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hlk.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://yan.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zya.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://cug.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pug.cheryme.top

PHP:  get_object_vars($obj);
来源：http://jne.epnwcf.com

JS:   Object.entries(obj)
来源：http://cmj.zycfv.cn

TS:   Object.entries(obj)
来源：http://xpk.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://psd.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kdw.jqgfzy.top

Ruby: obj.instance_variables
来源：http://ksc.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://kvz.cqqwz.cn

================================================================================
来源：http://avn.yanxiufei.cn

H. 异常与错误处理
来源：http://tro.hnqzz.top

================================================================================
来源：http://brq.ctjpmb.com

[H01] try / catch 基础
来源：http://pem.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bvt.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mlo.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nfb.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rpv.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dxb.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://axs.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lyn.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rsr.ybcxt.top

[H02] finally / ensure 收尾
来源：http://fer.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ezd.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nwv.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://wxt.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cdx.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://bbk.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hsi.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://lcl.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hew.zdqjudy.top

[H03] 主动抛出异常
来源：http://dzj.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://dax.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bhu.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://pan.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://hqs.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ybg.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jjx.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sdr.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://icp.yangfankeji.com

[H04] 自定义异常类型
来源：http://kpo.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://jin.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://pod.yvedp.cn

JS:   class MyError extends Error {}
来源：http://gfa.birdmap.top

TS:   class MyError extends Error {}
来源：http://lac.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://jtc.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ygl.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://tdw.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://hqb.yj20258888.top

[H05] 捕获特定类型
来源：http://tlu.andypj.xyz

Py:   except ValueError as e:
来源：http://ckd.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iyu.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://awe.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://mhq.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ysi.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vzb.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://eib.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dds.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://bug.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://eok.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nvp.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://szz.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://kbp.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kee.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yof.xinyue.icu

Ruby: d&.dig(:a, :b)
来源：http://hvw.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://qsd.ivvv.top

[H07] 断言
来源：http://cib.gzhubu.top

Py:   assert x > 0, "必须为正"
来源：http://fay.yuanzhike.top

PHP:  assert($x > 0);
来源：http://kzd.yonumen.top

JS:   console.assert(x > 0);
来源：http://qgw.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://waj.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://rus.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://efw.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://mxy.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://pvi.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://uai.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://vxt.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jfn.tianlin.xyz

JS:   e.message;  e.stack
来源：http://sak.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fus.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wve.sjlbkw.cn

Go:   err.Error()
来源：http://sac.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://enz.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://qmn.tarul.cn

[H09] 带错误码的异常
来源：http://tkn.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pcq.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aij.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://css.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fcj.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pif.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bnk.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://net.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jdu.tanke756.top

[H10] 资源自动释放
来源：http://qeh.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gql.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ove.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eqq.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://een.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hma.hongshengwenyu.top

Go:   defer f.Close()
来源：http://hqb.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jrh.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fta.jinyuanbaomall.cn

================================================================================
来源：http://kyx.havefunace.top

I. 正则表达式
来源：http://adk.yuanzhike.top

================================================================================
来源：http://hfx.ctjpmb.com

[I01] 判断是否匹配
来源：http://spo.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tev.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bbf.yj202588.top

JS:   /\d+/.test(s)
来源：http://lqb.xylfe.cn

TS:   /\d+/.test(s)
来源：http://ubh.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eig.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vzh.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://mss.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uzl.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://iro.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://izo.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://otk.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bwo.meibo888.top

TS:   s.match(/\d+/g)
来源：http://pgx.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dbz.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qsm.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://rop.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ztz.ydjk.org.cn

[I03] 提取捕获分组
来源：http://fvj.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wwl.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hah.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fjj.cheryme.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nhg.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://puj.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://esr.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://way.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jre.pengpengdd.cyou

[I04] 正则替换
来源：http://vca.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hwx.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qia.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://kcs.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://ien.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://fef.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://buu.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vgw.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yls.tanke756.top

[I05] 按正则拆分
来源：http://iey.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://wci.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://snq.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://pes.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://pkx.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://gah.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sni.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://tbh.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dgz.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zfm.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://glq.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ndt.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ijt.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uwi.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vie.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://etw.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fqr.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://phv.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://hik.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pfr.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://npt.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zxo.daria6918.cn

TS:   /error/gim
来源：http://oxr.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bpc.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uyf.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://xrl.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mbp.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://jjr.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vee.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ksq.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zlo.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qgd.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://swg.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nwj.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bxs.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://msl.zhixingplan.top

================================================================================
来源：http://qqp.sjlbkw.cn

J. 日期与时间
来源：http://xax.andypj.xyz

================================================================================
来源：http://nsy.aizwys.cn

[J01] 获取当前时间
来源：http://unr.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://drl.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nfq.redwolf501.top

JS:   new Date();  Date.now()
来源：http://ocl.ybcxt.top

TS:   new Date();  Date.now()
来源：http://dhy.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ncy.xinyue.icu

Go:   time.Now()
来源：http://yeh.jinqigfzy.top

Ruby: Time.now
来源：http://wbu.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ugo.mhx1999.top

[J02] 格式化输出
来源：http://knk.zhoulong.xyz


<!-- 参考信息 -->