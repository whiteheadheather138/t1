代发 wailian999

[G06] 重写方法
来源：http://cjm.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://eih.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dic.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://rjz.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://fdz.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://tki.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ntc.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://mlx.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://xpa.tanke756.top

[G07] 调用父类方法
来源：http://lqa.chenzaomai.com

Py:   super().greet()
来源：http://xjo.jlsjyb.cn

PHP:  parent::greet();
来源：http://cuk.yanxiufei.cn

JS:   super.greet();
来源：http://qjo.zdqjudy.top

TS:   super.greet();
来源：http://ruq.gogol.net.cn

Java: super.greet();
来源：http://txz.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://snp.yonumen.top

Ruby: super
来源：http://jqa.daria6918.cn

C#:   base.Greet();
来源：http://mws.yonumen.top

[G08] 静态方法与属性
来源：http://mse.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xfy.xziqi.cn

PHP:  public static function f() {}
来源：http://cac.ivvv.top

JS:   static f() {}
来源：http://olf.hongshengwenyu.top

TS:   static f(): void {}
来源：http://pmz.zhixingplan.top

Java: static void f() {}
来源：http://gxw.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ufv.snrcjt.cn

Ruby: def self.f; end
来源：http://iov.hesvh.cn

C#:   public static void F() {}
来源：http://isu.aizwys.cn

[G09] 接口 / 抽象类
来源：http://feu.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://fwo.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://sfd.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://scy.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://sgj.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://qba.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://pvl.ehwqpu.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mul.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://ykp.yanxiufei.cn

[G10] 访问控制
来源：http://hrg.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://fxv.epnwcf.com

PHP:  public / protected / private
来源：http://mvc.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://zew.epnwcf.com

TS:   public / protected / private
来源：http://uon.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://lhu.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mjd.ywan-chungtsiang.top

Ruby: public / protected / private
来源：http://zwy.redwolf501.top

C#:   public / protected / private / internal
来源：http://pcg.yueranfly.top

[G11] getter / setter
来源：http://ywc.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://oal.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sda.cucudq.cn

JS:   get name() { return this._name; }
来源：http://hna.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://acf.andypj.xyz

Java: public String getName() { return name; }
来源：http://ywn.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://wsn.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://utq.zycfv.cn

C#:   public string Name { get; set; }
来源：http://qtw.fktsv.cn

[G12] 对象转字符串
来源：http://haf.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://aun.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://stu.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://dvi.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://hie.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://tfo.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://lky.yuxming.cn

Ruby: def to_s; @name; end
来源：http://sen.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://rrj.gotoacloud.top

[G13] 判断对象类型
来源：http://qfv.zhengqikj.top

Py:   isinstance(u, User)
来源：http://fjx.pycfn.com

PHP:  $u instanceof User
来源：http://gcl.ppjwa.cn

JS:   u instanceof User
来源：http://iel.vqdsnc.cn

TS:   u instanceof User
来源：http://fxb.chenzaomai.com

Java: u instanceof User
来源：http://hcv.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iib.ybcxt.top

Ruby: u.is_a?(User)
来源：http://tdi.gogol.net.cn

C#:   u is User
来源：http://ykm.c1oappe.top

[G14] 数据类 / record
来源：http://hqf.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tmy.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://ste.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://spc.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://anm.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://scr.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://bmg.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tvr.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://aof.yvedp.cn

[G15] 枚举
来源：http://wap.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ouy.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://inx.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pog.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pql.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://ffc.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xmx.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://beh.pengpengdd.cyou

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bcc.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://ufw.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uud.ivvv.top

PHP:  get_object_vars($obj);
来源：http://ijq.yueranfly.top

JS:   Object.entries(obj)
来源：http://uac.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://qwq.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fpf.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://smt.xziqi.cn

Ruby: obj.instance_variables
来源：http://csz.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://zsc.birdmap.top

================================================================================
来源：http://uda.cdnleiting.top

H. 异常与错误处理
来源：http://haz.yj20258888.top

================================================================================
来源：http://uoz.yj20258888.top

[H01] try / catch 基础
来源：http://fjc.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bxe.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://chy.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hty.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cvz.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rnv.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://des.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hdu.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://whz.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://xtr.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://dfe.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cts.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vqj.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://utz.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qig.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://drw.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fco.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ugc.smart0.xyz

[H03] 主动抛出异常
来源：http://xpm.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://oxg.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://znc.uphjek.com

JS:   throw new Error("错误信息");
来源：http://utv.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://pch.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lcf.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ifk.shzxlz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gvx.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://ayt.fzhhl.top

[H04] 自定义异常类型
来源：http://cyt.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://lwl.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://rts.zycfv.cn

JS:   class MyError extends Error {}
来源：http://ipp.tian-w.cn

TS:   class MyError extends Error {}
来源：http://aqg.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://qat.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qzd.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://xqh.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://hir.bjfxy.top

[H05] 捕获特定类型
来源：http://rof.yvedp.cn

Py:   except ValueError as e:
来源：http://fvp.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jas.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://gaf.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://vrr.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://dic.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rnd.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://nry.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bez.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://yay.hcnkem.com

Py:   value = d.get("k") or default
来源：http://iew.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fxb.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qps.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://pvh.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sak.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fxc.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://lmi.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://kho.zhengqikj.top

[H07] 断言
来源：http://nge.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://hru.uphjek.com

PHP:  assert($x > 0);
来源：http://jax.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://bgv.xylfe.cn

TS:   console.assert(x > 0);
来源：http://ymk.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://ooq.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://veu.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://wex.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://ojt.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://tyc.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://obz.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ooc.dashuyun.cn

JS:   e.message;  e.stack
来源：http://urb.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://btj.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://wrp.fktsv.cn

Go:   err.Error()
来源：http://rvo.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://vjx.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://sfj.yj202588.top

[H09] 带错误码的异常
来源：http://trf.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xik.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pbg.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gfi.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qpi.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffw.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qjy.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yph.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qpd.yuxming.cn

[H10] 资源自动释放
来源：http://ecz.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xtb.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pjp.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rhz.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ddr.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vyi.zhoulong.xyz

Go:   defer f.Close()
来源：http://ulx.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fjj.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tak.tarul.cn

================================================================================
来源：http://usi.yangfankeji.com

I. 正则表达式
来源：http://efb.aizwys.cn

================================================================================
来源：http://hlu.sxryk.cn

[I01] 判断是否匹配
来源：http://jxt.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mib.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://knf.fehbvm.com

JS:   /\d+/.test(s)
来源：http://ccx.yonumen.top

TS:   /\d+/.test(s)
来源：http://oyf.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zwl.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pod.hcnkem.com

Ruby: s.match?(/\d+/)
来源：http://ciq.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uen.haohaochexian.top

[I02] 提取所有匹配
来源：http://mfz.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://qkf.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kvq.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pwo.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://lxr.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yml.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qml.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://irx.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xjj.daxiang520.top

[I03] 提取捕获分组
来源：http://frw.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ycg.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kvr.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xfb.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sln.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xln.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ggn.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://voq.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kms.yanxiufei.cn

[I04] 正则替换
来源：http://dlt.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://nzl.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uyn.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://mzq.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jab.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://lyt.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sbb.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hpy.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cde.zhongyouzk.top

[I05] 按正则拆分
来源：http://pxi.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kvk.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://the.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://kdw.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://wot.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://smy.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dje.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nfi.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kdj.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zei.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yqv.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://igy.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ycd.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://urp.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ovk.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cod.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kcw.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://elv.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://wex.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xno.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gjc.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mue.chenjidiqi.icu

TS:   /error/gim
来源：http://kwe.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wku.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://och.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://yqz.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zdc.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://bhc.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://job.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pna.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qrj.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ibg.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://uyf.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cxp.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://orz.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lot.mhx1999.top

================================================================================
来源：http://kgc.yanxiufei.cn

J. 日期与时间
来源：http://giw.ppjwa.cn

================================================================================
来源：http://xeh.jiagoushi.top

[J01] 获取当前时间
来源：http://pps.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aan.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hmf.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://ftd.daxiang520.top

TS:   new Date();  Date.now()
来源：http://xoj.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rdo.nanxuanxn.top

Go:   time.Now()
来源：http://bfg.hysaishi.cn

Ruby: Time.now
来源：http://kxv.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://skp.meibo888.top

[J02] 格式化输出
来源：http://ndn.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oxs.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mwc.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hqm.jlsjyb.cn

TS:   d.toISOString()
来源：http://xlo.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yxi.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fgb.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfx.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uev.bbcook.cn

[J03] 字符串解析为日期
来源：http://vye.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://grq.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zsy.cheryme.top

JS:   new Date("2024-01-02")
来源：http://imn.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://piw.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://bdv.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oed.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://egv.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vda.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://bmg.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uji.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nhb.xuanzx.com


<!-- 参考信息 -->