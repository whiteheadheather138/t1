代发 wailian999

Py:   class Admin(User): pass
来源：http://mdh.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://ocq.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://pjp.hfpthk.cn

TS:   class Admin extends User {}
来源：http://whc.birdmap.top

Java: class Admin extends User {}
来源：http://tqs.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hsm.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://nxb.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://cif.fktsv.cn

[G06] 重写方法
来源：http://soy.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://yfe.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kgg.yj202588.top

JS:   greet() { return "admin"; }
来源：http://bnl.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://sre.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://ftz.wangshuangyany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hul.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://awf.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://xvx.kuanghao11.cn

[G07] 调用父类方法
来源：http://zkn.chenzaomai.com

Py:   super().greet()
来源：http://eee.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://znb.hongshengwenyu.top

JS:   super.greet();
来源：http://nwj.hnxiangtu.top

TS:   super.greet();
来源：http://iih.ybcxt.top

Java: super.greet();
来源：http://idf.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aik.yvedp.cn

Ruby: super
来源：http://hgx.fengsongda.top

C#:   base.Greet();
来源：http://bcx.aizwys.cn

[G08] 静态方法与属性
来源：http://nmd.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zac.zhoulong.xyz

PHP:  public static function f() {}
来源：http://pgk.yvedp.cn

JS:   static f() {}
来源：http://xen.xuetiantiany.cn

TS:   static f(): void {}
来源：http://atu.yonumen.top

Java: static void f() {}
来源：http://xty.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ztb.haohaochexian.top

Ruby: def self.f; end
来源：http://rpp.xziqi.cn

C#:   public static void F() {}
来源：http://ont.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://tnx.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://igo.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://rym.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ykx.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://kxt.vehdjk.com

Java: interface Shape { double area(); }
来源：http://alt.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://msy.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mnn.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://rpc.yongpay.top

[G10] 访问控制
来源：http://utc.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://klh.guannengcc.top

PHP:  public / protected / private
来源：http://dsi.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://css.epnwcf.com

TS:   public / protected / private
来源：http://jwp.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://pjm.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://swi.zhiwuduotai.top

Ruby: public / protected / private
来源：http://cre.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://hni.cqqwz.cn

[G11] getter / setter
来源：http://zab.sysykeji.top

Py:   @property 与 @x.setter
来源：http://pow.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jqe.yonumen.top

JS:   get name() { return this._name; }
来源：http://eht.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://nsq.jinyuanbaomall.cn

Java: public String getName() { return name; }
来源：http://czy.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uyw.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://uyr.havefunace.top

C#:   public string Name { get; set; }
来源：http://qop.ydzc1.top

[G12] 对象转字符串
来源：http://knv.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://aik.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ezu.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://xme.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://fkc.sweek.top

Java: @Override public String toString() { return name; }
来源：http://xwe.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rlg.sysykeji.top

Ruby: def to_s; @name; end
来源：http://ccv.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://efa.chenjidiqi.icu

[G13] 判断对象类型
来源：http://kka.daria6918.cn

Py:   isinstance(u, User)
来源：http://jdg.yj202588.top

PHP:  $u instanceof User
来源：http://efl.nwbrower.top

JS:   u instanceof User
来源：http://loy.kuanghao11.cn

TS:   u instanceof User
来源：http://afp.jqgufenzy.top

Java: u instanceof User
来源：http://xaj.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dzm.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://jtm.nanxuanxn.top

C#:   u is User
来源：http://grb.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://ykt.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uof.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://qtq.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://ory.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://zll.bjfxy.top

Java: record User(String name, int age) {}
来源：http://xwm.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://pqf.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pep.cashguo.top

C#:   record User(string Name, int Age);
来源：http://lzg.jinqigfzy.top

[G15] 枚举
来源：http://vor.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bht.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pcm.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lcw.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hfv.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://bgy.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://whu.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://bhh.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jmb.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://vui.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qdj.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://zso.xziqi.cn

JS:   Object.entries(obj)
来源：http://xxl.daxiang520.top

TS:   Object.entries(obj)
来源：http://has.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aqa.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://fcb.epnwcf.com

Ruby: obj.instance_variables
来源：http://wrp.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://eot.jqgfzy.top

================================================================================
来源：http://hxu.yongpay.top

H. 异常与错误处理
来源：http://gnv.epnwcf.com

================================================================================
来源：http://aia.cucudq.cn

[H01] try / catch 基础
来源：http://lol.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wtx.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blt.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nur.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rvq.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://afp.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://udl.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gus.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ite.tarul.cn

[H02] finally / ensure 收尾
来源：http://ati.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://ifj.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nqg.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dkw.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xdo.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xtp.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xar.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vft.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nze.haohaochexian.top

[H03] 主动抛出异常
来源：http://lbw.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://lgg.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wxp.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://dsr.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://mzq.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://act.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cuv.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rlq.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fhi.dashuyun.cn

[H04] 自定义异常类型
来源：http://owf.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://hoe.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cri.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://fcs.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://iea.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://xrp.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kko.tanke756.top

Ruby: class MyError < StandardError; end
来源：http://vfj.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://tmy.jinqigfzy.top

[H05] 捕获特定类型
来源：http://adl.nanxinkj.top

Py:   except ValueError as e:
来源：http://dph.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://svx.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://goz.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://tzr.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://gvg.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rgt.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://uvi.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nby.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://ifb.guannengcc.top

Py:   value = d.get("k") or default
来源：http://ast.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://ngz.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uiy.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tad.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mzr.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fkw.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://zhq.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://nem.yj202588.top

[H07] 断言
来源：http://ldh.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://tqv.tian-w.cn

PHP:  assert($x > 0);
来源：http://dqj.shuidangran.top

JS:   console.assert(x > 0);
来源：http://hsk.cheryme.top

TS:   console.assert(x > 0);
来源：http://ucw.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://vaj.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jyw.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://evm.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://fku.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://yqu.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://odf.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://haz.redwolf501.top

JS:   e.message;  e.stack
来源：http://tvf.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dom.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://onc.vehdjk.com

Go:   err.Error()
来源：http://sbf.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://qdy.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://ejc.jiagoushi.top

[H09] 带错误码的异常
来源：http://bec.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tbd.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ehh.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dcr.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://slz.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wro.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mlv.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://nzs.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ntg.iojbl.cn

[H10] 资源自动释放
来源：http://aox.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mox.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gfa.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kpx.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uku.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qkw.xziqi.cn

Go:   defer f.Close()
来源：http://cgj.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ldi.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hqy.shuidangran.top

================================================================================
来源：http://xcw.cdnleiting.top

I. 正则表达式
来源：http://dax.guowangkeji.top

================================================================================
来源：http://zwd.snrcjt.cn

[I01] 判断是否匹配
来源：http://fzl.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jps.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://tkb.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://oui.yvedp.cn

TS:   /\d+/.test(s)
来源：http://ldu.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bgw.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hbn.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://onn.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rab.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://cbq.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://him.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://khu.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ctt.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://axv.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zbr.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hge.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://okr.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bct.chenlongwang.top

[I03] 提取捕获分组
来源：http://khm.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://erz.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uzc.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mln.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sdo.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wor.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dfz.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://djd.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fwd.quarkkingdee.top

[I04] 正则替换
来源：http://edk.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zth.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://djn.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fof.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mpw.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lvb.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dsz.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://clk.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vmd.cheryme.top

[I05] 按正则拆分
来源：http://cnv.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://hbg.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gfg.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://ouc.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://oag.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://dwi.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sbb.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://vam.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://trc.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://djb.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xuf.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xtf.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rjq.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://etw.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jgq.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ony.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kwx.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://elv.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://kgo.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pta.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oks.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://usa.wangshuangyany.cn

TS:   /error/gim
来源：http://ffu.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wwc.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cgj.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://tlr.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://azy.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://lfk.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kkg.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kei.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nkc.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sec.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://blp.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ouh.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hka.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fdb.fktsv.cn

================================================================================
来源：http://rgq.wangdashe.top

J. 日期与时间
来源：http://knn.tianlin.xyz

================================================================================
来源：http://cug.hesvh.cn

[J01] 获取当前时间
来源：http://nih.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nkt.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jsp.xinyue.icu

JS:   new Date();  Date.now()
来源：http://sud.iojbl.cn

TS:   new Date();  Date.now()
来源：http://hia.chenjidiqi.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://hfl.zhengqikj.top

Go:   time.Now()
来源：http://evk.ybcxt.top

Ruby: Time.now
来源：http://cty.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aod.shzxlz.cn

[J02] 格式化输出
来源：http://rqg.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lti.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gnk.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ocx.jyoumei.cn

TS:   d.toISOString()
来源：http://rmr.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cvv.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fep.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gnk.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wbh.guannengcc.top

[J03] 字符串解析为日期
来源：http://rdj.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cbp.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zvu.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://std.hesvh.cn


<!-- 参考信息 -->