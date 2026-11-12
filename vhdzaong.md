代发 wailian999

[G06] 重写方法
来源：http://lxb.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://pux.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ewh.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://ptl.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://ivd.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://lno.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yyo.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://kti.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://rjb.nanxuanxn.top

[G07] 调用父类方法
来源：http://bss.xinyue.icu

Py:   super().greet()
来源：http://qys.wangdashe.top

PHP:  parent::greet();
来源：http://zgf.wangshuangyany.cn

JS:   super.greet();
来源：http://qlo.nanxinkj.top

TS:   super.greet();
来源：http://jvx.zhiwuduotai.top

Java: super.greet();
来源：http://kpb.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://han.redwolf501.top

Ruby: super
来源：http://eyw.fktsv.cn

C#:   base.Greet();
来源：http://dud.52xcode.cn

[G08] 静态方法与属性
来源：http://zcq.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qfn.hnqzz.top

PHP:  public static function f() {}
来源：http://ykh.yfazqb.com

JS:   static f() {}
来源：http://dbl.zhiwuduotai.top

TS:   static f(): void {}
来源：http://yif.epnwcf.com

Java: static void f() {}
来源：http://vpg.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cwx.havefunace.top

Ruby: def self.f; end
来源：http://kvh.zdqjudy.top

C#:   public static void F() {}
来源：http://isj.redwolf501.top

[G09] 接口 / 抽象类
来源：http://ygv.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://ggw.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://rrc.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ibz.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://pcp.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://ght.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://nbp.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qfy.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://ewj.iojbl.cn

[G10] 访问控制
来源：http://uwi.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://icy.meibo888.top

PHP:  public / protected / private
来源：http://url.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://ytr.epnwcf.com

TS:   public / protected / private
来源：http://mos.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://dqw.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sqp.andypj.xyz

Ruby: public / protected / private
来源：http://ttf.yongpay.top

C#:   public / protected / private / internal
来源：http://zcv.hnqzz.top

[G11] getter / setter
来源：http://gat.xuanzx.com

Py:   @property 与 @x.setter
来源：http://yse.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wga.hnqzz.top

JS:   get name() { return this._name; }
来源：http://vvg.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://vdp.havefunace.top

Java: public String getName() { return name; }
来源：http://qbu.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ruu.zycfv.cn

Ruby: attr_accessor :name
来源：http://zfk.hcnkem.com

C#:   public string Name { get; set; }
来源：http://qja.dashuyun.cn

[G12] 对象转字符串
来源：http://yhe.ivvv.top

Py:   def __str__(self): return self.name
来源：http://add.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dox.fehbvm.com

JS:   toString() { return this.name; }
来源：http://rbr.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://kmt.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://ovl.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://pte.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://tjd.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://ymj.xinyue.icu

[G13] 判断对象类型
来源：http://rzf.dashuyun.cn

Py:   isinstance(u, User)
来源：http://sag.yuanzhike.top

PHP:  $u instanceof User
来源：http://iqo.birdmap.top

JS:   u instanceof User
来源：http://bzi.dashuyun.cn

TS:   u instanceof User
来源：http://tbx.ehwqpu.com

Java: u instanceof User
来源：http://lxw.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eyl.bjfxy.top

Ruby: u.is_a?(User)
来源：http://aai.ctjpmb.com

C#:   u is User
来源：http://gaf.gzhubu.top

[G14] 数据类 / record
来源：http://ntv.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vlb.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://lyz.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dxa.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://phs.ivvv.top

Java: record User(String name, int age) {}
来源：http://sgi.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://llb.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gfr.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://qxz.zdbjq.cn

[G15] 枚举
来源：http://dzq.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vrv.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vfm.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://opz.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ytl.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://mxe.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kgb.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://tvt.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pos.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://qsy.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vid.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://fsl.yvedp.cn

JS:   Object.entries(obj)
来源：http://uxc.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://mxx.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vpc.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hlx.yj20258.top

Ruby: obj.instance_variables
来源：http://oiw.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://iul.redwolf501.top

================================================================================
来源：http://syt.yonumen.top

H. 异常与错误处理
来源：http://fdg.tianlin.xyz

================================================================================
来源：http://ljl.iojbl.cn

[H01] try / catch 基础
来源：http://ljk.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kao.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://exf.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pwt.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://brl.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pox.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://brj.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fyh.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tzm.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://lde.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://fbl.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kik.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cle.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://zrz.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://chi.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ywa.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kuv.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nrm.yj20258.top

[H03] 主动抛出异常
来源：http://kcj.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://qdd.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dyz.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://qcc.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://kgb.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qav.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://awv.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qns.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://wlf.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://whx.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://tmc.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://fli.zycfv.cn

JS:   class MyError extends Error {}
来源：http://qsx.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://xow.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://kif.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qcq.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://xaz.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://xrz.fengsongda.top

[H05] 捕获特定类型
来源：http://pkm.bjfxy.top

Py:   except ValueError as e:
来源：http://kwm.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uqh.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://wrj.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://kpa.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://klm.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uer.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://bck.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jal.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://irv.aizwys.cn

Py:   value = d.get("k") or default
来源：http://zbb.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://dey.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://oql.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bqg.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ccq.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qxb.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://ahk.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://kmk.birdmap.top

[H07] 断言
来源：http://xoj.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://cbw.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://obw.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://osz.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://ekk.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://xbz.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://omt.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://euu.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://avo.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://fbu.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://zmy.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vcf.wangdashe.top

JS:   e.message;  e.stack
来源：http://bwx.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ark.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uwo.sysykeji.top

Go:   err.Error()
来源：http://ufq.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://rhz.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://iqy.gogol.net.cn

[H09] 带错误码的异常
来源：http://rme.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qno.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gig.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://txo.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nmq.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lyb.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xrx.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://jjw.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uwb.zdbjq.cn

[H10] 资源自动释放
来源：http://aey.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fqm.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qip.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qmt.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fzw.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dln.zhongyouzk.top

Go:   defer f.Close()
来源：http://kay.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oym.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ahi.9152youxi.cn

================================================================================
来源：http://gqu.wangshuangyany.cn

I. 正则表达式
来源：http://zle.fengsongda.top

================================================================================
来源：http://nci.chenzaomai.com

[I01] 判断是否匹配
来源：http://qmr.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ieo.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://dwg.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://hul.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://zip.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bui.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ryy.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://vfr.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zqx.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://mhr.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://wuy.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://anj.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jbh.tanke756.top

TS:   s.match(/\d+/g)
来源：http://aua.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://btk.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sca.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://nvz.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qak.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://atv.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pem.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mzy.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jwc.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kpn.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rbi.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xbn.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fir.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nij.hfpthk.cn

[I04] 正则替换
来源：http://cqz.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iof.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gfa.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://ppg.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://het.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mjk.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://htd.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nwx.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vny.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://fxj.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ygk.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://drt.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://jdf.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://kpk.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://kca.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uri.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://grd.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://twe.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zaz.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fiy.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wtl.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cvs.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lqm.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wug.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ylt.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://evi.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wti.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://mvx.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oct.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pru.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vfg.nwbrower.top

TS:   /error/gim
来源：http://dyk.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ijx.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zhb.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://hff.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ofd.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://pkf.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lfb.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sqp.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://syv.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zoh.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wxw.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ozt.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hfe.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://prw.cheryme.top

================================================================================
来源：http://rea.fktsv.cn

J. 日期与时间
来源：http://hcf.jianghu66.top

================================================================================
来源：http://pzf.pengpengdd.cyou

[J01] 获取当前时间
来源：http://wzz.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ovd.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://myr.hcnkem.com

JS:   new Date();  Date.now()
来源：http://fkd.yfazqb.com

TS:   new Date();  Date.now()
来源：http://kmz.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qvg.ppjwa.cn

Go:   time.Now()
来源：http://ymb.xuanzx.com

Ruby: Time.now
来源：http://ibc.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kod.jlsjyb.cn

[J02] 格式化输出
来源：http://hos.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hgv.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hab.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xsj.hcnkem.com

TS:   d.toISOString()
来源：http://bys.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wyg.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ist.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lqm.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://puw.guowangkeji.top

[J03] 字符串解析为日期
来源：http://qwu.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oes.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mvn.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://vxv.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://bbv.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yny.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dgb.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://aby.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tmt.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://sgg.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://amv.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eqf.hnxiangtu.top


<!-- 参考信息 -->