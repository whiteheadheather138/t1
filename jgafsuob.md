代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://zfm.zhixingplan.top

Ruby: def greet; @name; end
来源：http://zwj.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://phg.tianlin.xyz

[G05] 继承
来源：http://hkt.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://pwf.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://gkg.fktsv.cn

JS:   class Admin extends User {}
来源：http://hte.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://klq.ctjpmb.com

Java: class Admin extends User {}
来源：http://amj.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lry.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://dxv.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://nsl.dashuyun.cn

[G06] 重写方法
来源：http://vkm.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://pqw.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://peq.sweek.top

JS:   greet() { return "admin"; }
来源：http://exh.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://vqw.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://uwc.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://adf.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://jva.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://xhk.jyoumei.cn

[G07] 调用父类方法
来源：http://enh.birdmap.top

Py:   super().greet()
来源：http://uuw.hesvh.cn

PHP:  parent::greet();
来源：http://ddp.jinyuanbaomall.cn

JS:   super.greet();
来源：http://atb.daxiang520.top

TS:   super.greet();
来源：http://nyg.fzhhl.top

Java: super.greet();
来源：http://cyu.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oqq.yuxming.cn

Ruby: super
来源：http://zus.dashuyun.cn

C#:   base.Greet();
来源：http://pyy.sufxvd.cn

[G08] 静态方法与属性
来源：http://xad.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pvi.yj20258888.top

PHP:  public static function f() {}
来源：http://zjb.smart0.xyz

JS:   static f() {}
来源：http://xwz.hnxiangtu.top

TS:   static f(): void {}
来源：http://hpv.hcnkem.com

Java: static void f() {}
来源：http://pjf.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nrt.ydzc1.top

Ruby: def self.f; end
来源：http://scs.jqgfzy.top

C#:   public static void F() {}
来源：http://eig.gzhubu.top

[G09] 接口 / 抽象类
来源：http://erq.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://tvw.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dkv.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://loe.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://hjg.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://fst.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://mxa.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mbq.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://uei.kuanghao11.cn

[G10] 访问控制
来源：http://zeh.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://cmo.hammf.cn

PHP:  public / protected / private
来源：http://pzw.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://hyx.bjfxy.top

TS:   public / protected / private
来源：http://zxn.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://nnh.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ynl.yj20258888.top

Ruby: public / protected / private
来源：http://foc.xziqi.cn

C#:   public / protected / private / internal
来源：http://smd.gotoacloud.top

[G11] getter / setter
来源：http://vrh.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://wun.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ohq.ybcxt.top

JS:   get name() { return this._name; }
来源：http://juy.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://bjv.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://zxz.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hpi.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://pux.hammf.cn

C#:   public string Name { get; set; }
来源：http://vpv.birdmap.top

[G12] 对象转字符串
来源：http://ref.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://nyh.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kcv.bjfxy.top

JS:   toString() { return this.name; }
来源：http://ywh.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://kpx.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://aom.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://uhf.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://jdw.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://tgy.zdqjudy.top

[G13] 判断对象类型
来源：http://klw.chenlongwang.top

Py:   isinstance(u, User)
来源：http://dex.nwbrower.top

PHP:  $u instanceof User
来源：http://vkh.shangyingyoupin.top

JS:   u instanceof User
来源：http://xve.hcnkem.com

TS:   u instanceof User
来源：http://drq.hnxiangtu.top

Java: u instanceof User
来源：http://czo.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tjd.sweek.top

Ruby: u.is_a?(User)
来源：http://gpe.chenlongwang.top

C#:   u is User
来源：http://tkd.yanxiufei.cn

[G14] 数据类 / record
来源：http://dyq.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wov.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://qqn.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bca.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://fjn.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://idc.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://rnw.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uka.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://gpv.xingfuxueyuan.xyz

[G15] 枚举
来源：http://cmc.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oxj.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://heq.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://klq.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://onb.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://iqc.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ztl.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://suh.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mda.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://dqb.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xwz.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://dww.yj20258.top

JS:   Object.entries(obj)
来源：http://xxs.shuidangran.top

TS:   Object.entries(obj)
来源：http://upg.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xbr.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://niz.ydzc1.top

Ruby: obj.instance_variables
来源：http://gei.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://fco.wangdashe.top

================================================================================
来源：http://ifz.gaohongyu789.top

H. 异常与错误处理
来源：http://ssy.xziqi.cn

================================================================================
来源：http://bfd.wangdashe.top

[H01] try / catch 基础
来源：http://stx.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lkv.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mnd.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ism.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://icg.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pyx.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jym.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://swm.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ofw.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://mbo.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://ops.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://srt.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wtr.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iwq.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://dsb.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://azc.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://okg.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://yzl.kuanghao11.cn

[H03] 主动抛出异常
来源：http://qmf.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://fsr.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://igg.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://hya.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://vkl.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cva.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kve.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yws.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lkd.jqgufenzy.top

[H04] 自定义异常类型
来源：http://sbl.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://esl.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://zpb.tanke756.top

JS:   class MyError extends Error {}
来源：http://uec.andypj.xyz

TS:   class MyError extends Error {}
来源：http://mhg.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://jzg.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jlh.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://dul.cashguo.top

C#:   class MyException : Exception {}
来源：http://nww.uphjek.com

[H05] 捕获特定类型
来源：http://rlp.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://uff.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hxt.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://kyu.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://gjr.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://lfg.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wku.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://deh.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://auq.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://uhp.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://ucn.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://sqe.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rmm.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://vgn.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ain.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ygw.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://npt.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://lwq.sjlbkw.cn

[H07] 断言
来源：http://gdi.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://eux.yj202588.top

PHP:  assert($x > 0);
来源：http://tfa.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://vkq.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://amq.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://rcl.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ufz.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bra.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://fwq.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://yzo.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://iam.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ayb.shzxlz.cn

JS:   e.message;  e.stack
来源：http://drp.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yil.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://abk.xylfe.cn

Go:   err.Error()
来源：http://jbb.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://izc.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://ylj.316326.xyz

[H09] 带错误码的异常
来源：http://lsj.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qum.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kgr.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yek.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ate.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ccv.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wvc.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://zxx.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mso.jiagoushi.top

[H10] 资源自动释放
来源：http://ktr.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ane.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ysd.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ojn.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mkl.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://clk.52xcode.cn

Go:   defer f.Close()
来源：http://wrb.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uad.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xtj.guowangkeji.top

================================================================================
来源：http://aqv.gaohongyu789.top

I. 正则表达式
来源：http://bmj.jinyuanbaomall.cn

================================================================================
来源：http://hsb.cdnleiting.top

[I01] 判断是否匹配
来源：http://stu.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ghp.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fjj.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://due.hnqzz.top

TS:   /\d+/.test(s)
来源：http://tmg.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://scn.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dfz.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://orz.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ytz.nwbrower.top

[I02] 提取所有匹配
来源：http://gfm.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://yke.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wtq.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kym.pycfn.com

TS:   s.match(/\d+/g)
来源：http://qav.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://spn.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mal.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://eor.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ylb.fehbvm.com

[I03] 提取捕获分组
来源：http://lry.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xfo.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bil.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mye.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://abu.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://olx.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kch.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zrw.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wkv.cqqwz.cn

[I04] 正则替换
来源：http://wzp.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://orc.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjf.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://itj.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://anz.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fav.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hvd.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xfv.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zjd.sweek.top

[I05] 按正则拆分
来源：http://rlz.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ywu.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vqx.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://qew.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://lps.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://tqt.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kdu.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://svt.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pod.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://utk.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pxt.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oyh.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jrm.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lbf.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://urp.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wsj.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zxo.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ddc.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://xpz.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bpz.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cdc.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bbh.hywenlv.cn

TS:   /error/gim
来源：http://oqz.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lkc.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wxv.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://uez.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rpd.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://ipo.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lwz.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zyr.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jct.zhongyouzk.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uig.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cll.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oju.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fkd.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pkj.jinqigufen.top

================================================================================
来源：http://vff.ctjpmb.com

J. 日期与时间
来源：http://skl.pengpengdd.cyou

================================================================================
来源：http://fqx.gaohongyu789.top

[J01] 获取当前时间
来源：http://vqr.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qdk.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sgx.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://mzx.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://kkj.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://psv.gzhubu.top

Go:   time.Now()
来源：http://tyb.yanxiufei.cn

Ruby: Time.now
来源：http://abz.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oga.zhijiandao.cn

[J02] 格式化输出
来源：http://vam.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mju.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://onf.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nkj.gzhubu.top

TS:   d.toISOString()
来源：http://hhz.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://evc.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nxv.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xkq.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://opp.jqgfzy.top


<!-- 参考信息 -->