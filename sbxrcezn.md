代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://dwu.sweek.top

JS:   greet() { return this.name; }
来源：http://dhs.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://ptr.fzhhl.top

Java: String greet() { return name; }
来源：http://bxa.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kux.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://dsm.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://wpv.zhongyouzk.top

[G05] 继承
来源：http://vxg.birdmap.top

Py:   class Admin(User): pass
来源：http://uqt.bbcook.cn

PHP:  class Admin extends User {}
来源：http://euz.yongpay.top

JS:   class Admin extends User {}
来源：http://fst.wangdashe.top

TS:   class Admin extends User {}
来源：http://taz.chenzaomai.com

Java: class Admin extends User {}
来源：http://fni.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://spf.uphjek.com

Ruby: class Admin < User; end
来源：http://tzs.snrcjt.cn

C#:   class Admin : User {}
来源：http://zoq.mhx1999.top

[G06] 重写方法
来源：http://bgd.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://xso.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://okg.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://bna.bjfxy.top

TS:   greet(): string { return "admin"; }
来源：http://teq.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://yil.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nse.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://jgj.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://vok.hongshengwenyu.top

[G07] 调用父类方法
来源：http://iae.yonumen.top

Py:   super().greet()
来源：http://ngh.zhixingplan.top

PHP:  parent::greet();
来源：http://ntk.tarul.cn

JS:   super.greet();
来源：http://the.meibo888.top

TS:   super.greet();
来源：http://uvg.shzxlz.cn

Java: super.greet();
来源：http://yjf.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hep.sxryk.cn

Ruby: super
来源：http://avl.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://mss.xylfe.cn

[G08] 静态方法与属性
来源：http://mnc.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ext.gzhubu.top

PHP:  public static function f() {}
来源：http://zti.zhiwuduotai.top

JS:   static f() {}
来源：http://qus.nanxinkj.top

TS:   static f(): void {}
来源：http://gri.zycfv.cn

Java: static void f() {}
来源：http://pgx.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kjg.nwbrower.top

Ruby: def self.f; end
来源：http://qia.svipenyu.cn

C#:   public static void F() {}
来源：http://ppc.ydzc1.top

[G09] 接口 / 抽象类
来源：http://kef.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://uvt.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hnp.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xdh.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://trt.shuidangran.top

Java: interface Shape { double area(); }
来源：http://poy.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://num.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qry.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://vxi.andypj.xyz

[G10] 访问控制
来源：http://uhu.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://mxq.bbcook.cn

PHP:  public / protected / private
来源：http://osj.52xcode.cn

JS:   #private 字段；其余公开
来源：http://ubg.jinqigufen.top

TS:   public / protected / private
来源：http://mwh.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://mdi.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uaj.52xcode.cn

Ruby: public / protected / private
来源：http://ago.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://iqc.yj20258888.top

[G11] getter / setter
来源：http://ifs.fehbvm.com

Py:   @property 与 @x.setter
来源：http://uhe.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://kcv.yuxming.cn

JS:   get name() { return this._name; }
来源：http://inx.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://ebm.fzhhl.top

Java: public String getName() { return name; }
来源：http://ygr.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wns.gzhubu.top

Ruby: attr_accessor :name
来源：http://vtt.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://blg.jlsjyb.cn

[G12] 对象转字符串
来源：http://ljl.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://dyb.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ido.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://gph.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://tqw.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://djo.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://yrw.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://whz.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://qtz.hongshengwenyu.top

[G13] 判断对象类型
来源：http://hqs.tarul.cn

Py:   isinstance(u, User)
来源：http://khx.gzhubu.top

PHP:  $u instanceof User
来源：http://upa.aizwys.cn

JS:   u instanceof User
来源：http://qag.yj20258.top

TS:   u instanceof User
来源：http://sfy.mhx1999.top

Java: u instanceof User
来源：http://mpi.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kui.cucudq.cn

Ruby: u.is_a?(User)
来源：http://tvm.shuidangran.top

C#:   u is User
来源：http://iqo.fzhhl.top

[G14] 数据类 / record
来源：http://ixl.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tdz.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://vor.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hvr.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://trv.c1oappe.top

Java: record User(String name, int age) {}
来源：http://ccn.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://xfs.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hig.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://txm.dianchejie.cn

[G15] 枚举
来源：http://xly.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jmq.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fmv.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vxy.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zff.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://oow.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lah.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://isa.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dxo.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://kzq.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hwv.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://xwl.yongpay.top

JS:   Object.entries(obj)
来源：http://kst.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://wst.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ipq.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://gjg.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://kfy.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://fph.hfpthk.cn

================================================================================
来源：http://zka.tarul.cn

H. 异常与错误处理
来源：http://qeg.zhoulong.xyz

================================================================================
来源：http://rix.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://jlg.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jzd.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hlg.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cpa.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zzs.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gzy.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://feq.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://frk.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ccs.smart0.xyz

[H02] finally / ensure 收尾
来源：http://rcm.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://vtx.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pos.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://oub.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zge.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vom.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://idf.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hqg.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pqz.meibo888.top

[H03] 主动抛出异常
来源：http://imr.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://gpe.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fuf.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://xut.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://xfs.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jci.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qoj.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://noo.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://huh.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://npx.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://eas.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wpj.daria6918.cn

JS:   class MyError extends Error {}
来源：http://akf.hcnkem.com

TS:   class MyError extends Error {}
来源：http://ynv.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://gxs.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hme.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://tsa.yj202588.top

C#:   class MyException : Exception {}
来源：http://imb.ehwqpu.com

[H05] 捕获特定类型
来源：http://lkm.nanxuanxn.top

Py:   except ValueError as e:
来源：http://cvk.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tfs.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://viq.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://ise.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://wkp.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xqu.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://urk.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tfu.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://ztw.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://fvv.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://nwh.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://jvt.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dvu.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cxv.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hvl.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://cav.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://woh.jinghuilouyu.cn

[H07] 断言
来源：http://sjl.fanxiaobao.xyz

Py:   assert x > 0, "必须为正"
来源：http://pek.yj20258888.top

PHP:  assert($x > 0);
来源：http://fxw.fktsv.cn

JS:   console.assert(x > 0);
来源：http://gca.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://qpj.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://axu.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wmo.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://crf.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://bqx.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://tsf.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://bho.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wjp.redwolf501.top

JS:   e.message;  e.stack
来源：http://aup.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lql.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hsz.aibaodan.cn

Go:   err.Error()
来源：http://ato.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://jtj.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://kxm.jianghu66.top

[H09] 带错误码的异常
来源：http://ltm.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qwc.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://otm.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mfj.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://clv.andypj.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rkb.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ikw.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vnd.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hss.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://gbj.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ekn.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rhn.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jzn.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qcq.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xrg.svipenyu.cn

Go:   defer f.Close()
来源：http://ngm.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kzf.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hge.jinqigufen.top

================================================================================
来源：http://dov.guannengcc.top

I. 正则表达式
来源：http://eiy.ivvv.top

================================================================================
来源：http://ucl.daxiang520.top

[I01] 判断是否匹配
来源：http://vjc.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wxf.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://olg.wangdashe.top

JS:   /\d+/.test(s)
来源：http://qgh.bjfxy.top

TS:   /\d+/.test(s)
来源：http://shk.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tid.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dmi.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://mxu.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zst.xinyue.icu

[I02] 提取所有匹配
来源：http://kep.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://grx.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cev.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cqg.yj20258.top

TS:   s.match(/\d+/g)
来源：http://ouz.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mci.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://grf.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://tbz.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mks.smart0.xyz

[I03] 提取捕获分组
来源：http://hgb.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ujj.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uwk.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gcv.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://klo.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wfz.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lim.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rcw.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dfk.xziqi.cn

[I04] 正则替换
来源：http://efk.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gey.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://clq.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kla.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cfu.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://tts.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://njp.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://rtx.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kky.fengsongda.top

[I05] 按正则拆分
来源：http://qpf.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ygp.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zcw.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://usm.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://die.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://ntw.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://njk.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://qre.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ngy.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wmz.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gqv.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://avl.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hqk.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://afo.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nmz.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pig.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://voz.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sxn.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://kcf.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zas.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rvw.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lui.yj202588.top

TS:   /error/gim
来源：http://vhr.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rdq.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ywl.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://qpu.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ruh.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://ijf.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cxc.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lud.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://boh.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://npr.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://mkh.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ayu.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dbv.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jyo.gogol.net.cn

================================================================================
来源：http://ckj.tianlin.xyz

J. 日期与时间
来源：http://tej.yfazqb.com

================================================================================
来源：http://zlw.sufxvd.cn

[J01] 获取当前时间
来源：http://xxm.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yop.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://smb.pycfn.com

JS:   new Date();  Date.now()
来源：http://esh.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://gej.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cnm.tian-w.cn

Go:   time.Now()
来源：http://lzt.hcnkem.com

Ruby: Time.now
来源：http://orp.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bjq.guowangkeji.top

[J02] 格式化输出
来源：http://rkn.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pvs.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kye.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xod.quarkkingdee.top

TS:   d.toISOString()
来源：http://qnw.snrcjt.cn


<!-- 参考信息 -->