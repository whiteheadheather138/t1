代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://abe.shangyingyoupin.top

[G07] 调用父类方法
来源：http://lil.sxryk.cn

Py:   super().greet()
来源：http://ouz.uphjek.com

PHP:  parent::greet();
来源：http://cxy.yongpay.top

JS:   super.greet();
来源：http://rrh.yfazqb.com

TS:   super.greet();
来源：http://miw.xinyue.icu

Java: super.greet();
来源：http://xrp.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://thi.hnxiangtu.top

Ruby: super
来源：http://tcg.cucudq.cn

C#:   base.Greet();
来源：http://ztz.52xcode.cn

[G08] 静态方法与属性
来源：http://pnv.xinyue.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dug.zdbjq.cn

PHP:  public static function f() {}
来源：http://cze.cqqwz.cn

JS:   static f() {}
来源：http://exf.vqdsnc.cn

TS:   static f(): void {}
来源：http://xab.zhiwuduotai.top

Java: static void f() {}
来源：http://uth.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zor.zhongyouzk.top

Ruby: def self.f; end
来源：http://qfb.svipenyu.cn

C#:   public static void F() {}
来源：http://thw.fehbvm.com

[G09] 接口 / 抽象类
来源：http://pff.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://zre.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nhk.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vop.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://yri.316326.xyz

Java: interface Shape { double area(); }
来源：http://fqd.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://clw.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jwh.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://ikb.guannengcc.top

[G10] 访问控制
来源：http://xpp.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ono.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://mbm.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://vrf.yueranfly.top

TS:   public / protected / private
来源：http://vsx.yongpay.top

Java: public / protected / private / 默认包级
来源：http://olg.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oht.ivvv.top

Ruby: public / protected / private
来源：http://aju.hcnkem.com

C#:   public / protected / private / internal
来源：http://zuc.ywan-chungtsiang.top

[G11] getter / setter
来源：http://wmn.yj202588.top

Py:   @property 与 @x.setter
来源：http://phr.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hzc.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://uxx.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://ocm.iojbl.cn

Java: public String getName() { return name; }
来源：http://wvy.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hjc.birdmap.top

Ruby: attr_accessor :name
来源：http://wjo.wangdashe.top

C#:   public string Name { get; set; }
来源：http://aqe.epnwcf.com

[G12] 对象转字符串
来源：http://flb.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://kxx.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kua.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://uuc.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://yle.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://mea.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://kew.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://qlw.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://ffn.yuxming.cn

[G13] 判断对象类型
来源：http://wpe.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://nnl.jqgfzy.top

PHP:  $u instanceof User
来源：http://vyk.nanxinkj.top

JS:   u instanceof User
来源：http://jmq.zdbjq.cn

TS:   u instanceof User
来源：http://rpt.ydjk.org.cn

Java: u instanceof User
来源：http://egs.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dra.daria6918.cn

Ruby: u.is_a?(User)
来源：http://jbg.yj20258888.top

C#:   u is User
来源：http://cqr.nwbrower.top

[G14] 数据类 / record
来源：http://qbv.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zfz.fktsv.cn

PHP:  // 用 readonly 属性模拟
来源：http://mnk.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://rqf.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://fup.bjfxy.top

Java: record User(String name, int age) {}
来源：http://gol.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://srg.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qpx.9152youxi.cn

C#:   record User(string Name, int Age);
来源：http://luj.xinyue.icu

[G15] 枚举
来源：http://dpa.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kuy.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://heu.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aka.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ysb.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://tra.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ijm.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://uqx.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gnz.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://com.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rbv.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://ywd.bjfxy.top

JS:   Object.entries(obj)
来源：http://gqh.birdmap.top

TS:   Object.entries(obj)
来源：http://ktb.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cik.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ews.uphjek.com

Ruby: obj.instance_variables
来源：http://jfx.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://rmo.ywan-chungtsiang.top

================================================================================
来源：http://iqq.chenjidiqi.icu

H. 异常与错误处理
来源：http://ocv.0kj1m.cn

================================================================================
来源：http://edh.sweek.top

[H01] try / catch 基础
来源：http://hcg.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cra.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rid.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qhd.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qlp.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jzw.aizwys.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oiy.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yzu.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lun.sysykeji.top

[H02] finally / ensure 收尾
来源：http://sjf.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vgf.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lvj.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zdz.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://gwn.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://ssk.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rib.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://knj.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sug.ctjpmb.com

[H03] 主动抛出异常
来源：http://lin.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://anu.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixw.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://qzi.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://gmr.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nos.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ohv.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rvm.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sha.zdqjudy.top

[H04] 自定义异常类型
来源：http://nvs.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://ghz.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hrs.tian-w.cn

JS:   class MyError extends Error {}
来源：http://cqt.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://mtz.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://qiw.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://heu.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://qbv.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://jjo.sxryk.cn

[H05] 捕获特定类型
来源：http://tim.gzhubu.top

Py:   except ValueError as e:
来源：http://hre.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tkx.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://fac.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://vws.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ssb.hywenlv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://miy.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://own.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zhd.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://bxx.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://egu.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://nid.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iac.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://xrs.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hdp.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eyw.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://jye.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://kgv.quarkkingdee.top

[H07] 断言
来源：http://ocy.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://cxl.guowangkeji.top

PHP:  assert($x > 0);
来源：http://caj.ybcxt.top

JS:   console.assert(x > 0);
来源：http://yza.epnwcf.com

TS:   console.assert(x > 0);
来源：http://ggz.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://leb.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xda.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://adw.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://fxf.sweek.top

[H08] 获取错误信息与堆栈
来源：http://hly.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://upi.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tqn.sxryk.cn

JS:   e.message;  e.stack
来源：http://ylp.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vnw.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://vsn.chenjidiqi.icu

Go:   err.Error()
来源：http://jeu.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://mvd.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://htj.chenlongwang.top

[H09] 带错误码的异常
来源：http://qvx.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vez.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mos.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mmb.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hzd.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rvf.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://foz.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nci.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://udq.fzhhl.top

[H10] 资源自动释放
来源：http://tlq.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rhg.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lsa.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yca.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fap.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fkk.redwolf501.top

Go:   defer f.Close()
来源：http://xvd.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vxb.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://usx.ehwqpu.com

================================================================================
来源：http://hjd.hammf.cn

I. 正则表达式
来源：http://rmy.zhengqikj.top

================================================================================
来源：http://wlr.yanxiufei.cn

[I01] 判断是否匹配
来源：http://ofh.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mif.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://wpd.fktsv.cn

JS:   /\d+/.test(s)
来源：http://uok.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://oli.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jyq.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bai.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://exx.zhijiandao.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dof.fzhhl.top

[I02] 提取所有匹配
来源：http://vmv.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://hjj.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://had.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vji.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://kka.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qsn.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wjh.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://ilf.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hyl.birdmap.top

[I03] 提取捕获分组
来源：http://saa.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bet.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://osg.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cjc.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ztz.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://utj.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fdi.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://myt.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ykv.ydzc1.top

[I04] 正则替换
来源：http://eqx.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rcw.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ndt.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://kpf.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://qyd.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://odt.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://jfw.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://skp.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bpt.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://rbk.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ukb.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dbt.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tzy.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://dvt.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://iqp.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tzp.tarul.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pdg.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://glt.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rbg.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://czy.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vas.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qxg.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kor.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iuv.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dtu.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kmi.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pqj.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://vnc.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ppd.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://edi.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oay.shanyushiyangtech.top

TS:   /error/gim
来源：http://ani.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://may.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cqs.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://cwx.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://omr.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://okd.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vrx.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://prn.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wuk.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ldd.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uey.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vts.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nno.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qio.sjlbkw.cn

================================================================================
来源：http://bpf.wangdashe.top

J. 日期与时间
来源：http://fzj.fktsv.cn

================================================================================
来源：http://bxr.cashguo.top

[J01] 获取当前时间
来源：http://ucm.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mot.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kkd.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://rys.epnwcf.com

TS:   new Date();  Date.now()
来源：http://cat.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zui.hysaishi.cn

Go:   time.Now()
来源：http://ens.ywan-chungtsiang.top

Ruby: Time.now
来源：http://rjj.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qgf.cheryme.top

[J02] 格式化输出
来源：http://twz.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://doj.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://azx.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wtm.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://lqv.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kfv.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bnv.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ajv.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vxm.cheryme.top

[J03] 字符串解析为日期
来源：http://hjg.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rdp.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bnv.yongpay.top

JS:   new Date("2024-01-02")
来源：http://rbk.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://kgh.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://ias.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://get.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://goo.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vav.yuxming.cn

[J04] 时间戳与日期互转
来源：http://wlm.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ytx.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fmc.zhoulong.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pag.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://rps.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ttk.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://snz.daria6918.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kgk.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://adl.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://tsa.tarul.cn

Py:   now + timedelta(days=7)
来源：http://zsv.bjfxy.top


<!-- 参考信息 -->