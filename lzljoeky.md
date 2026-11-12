代发 wailian999

[G06] 重写方法
来源：http://wcl.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://rwz.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bje.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://vje.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://vfz.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://hjz.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jvo.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://vnr.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://blz.haohaochexian.top

[G07] 调用父类方法
来源：http://glp.chenjidiqi.icu

Py:   super().greet()
来源：http://iuw.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://jfu.cheryme.top

JS:   super.greet();
来源：http://wvs.gotoacloud.top

TS:   super.greet();
来源：http://vgz.jyoumei.cn

Java: super.greet();
来源：http://xsh.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lig.dashuyun.cn

Ruby: super
来源：http://wpq.hammf.cn

C#:   base.Greet();
来源：http://ffp.epnwcf.com

[G08] 静态方法与属性
来源：http://anh.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rrf.tarul.cn

PHP:  public static function f() {}
来源：http://iek.xylfe.cn

JS:   static f() {}
来源：http://hdy.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://mxq.zhixingplan.top

Java: static void f() {}
来源：http://kzb.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ywd.guowangkeji.top

Ruby: def self.f; end
来源：http://flx.sysykeji.top

C#:   public static void F() {}
来源：http://fxo.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://zqm.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://gqb.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://hhi.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jcg.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://ppk.epnwcf.com

Java: interface Shape { double area(); }
来源：http://ibu.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://zfm.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://itg.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://zad.pengpengdd.cyou

[G10] 访问控制
来源：http://yza.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://tgd.chenjidiqi.icu

PHP:  public / protected / private
来源：http://uto.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://qju.daxiang520.top

TS:   public / protected / private
来源：http://wbt.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://ltj.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zhb.zhongyouzk.top

Ruby: public / protected / private
来源：http://wvj.ehwqpu.com

C#:   public / protected / private / internal
来源：http://ege.yonumen.top

[G11] getter / setter
来源：http://mgp.xylfe.cn

Py:   @property 与 @x.setter
来源：http://arr.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ubd.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://kkd.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://tty.tanke756.top

Java: public String getName() { return name; }
来源：http://oma.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fxp.sufxvd.cn

Ruby: attr_accessor :name
来源：http://qbi.xylfe.cn

C#:   public string Name { get; set; }
来源：http://ptf.zhixingplan.top

[G12] 对象转字符串
来源：http://ybd.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://yed.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ail.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://jkc.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://lxj.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://ysx.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://yuu.52xcode.cn

Ruby: def to_s; @name; end
来源：http://fqm.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://qxo.ivvv.top

[G13] 判断对象类型
来源：http://vev.yvedp.cn

Py:   isinstance(u, User)
来源：http://dhr.snrcjt.cn

PHP:  $u instanceof User
来源：http://cjk.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://fqz.jlsjyb.cn

TS:   u instanceof User
来源：http://fuw.birdmap.top

Java: u instanceof User
来源：http://pkd.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://kzd.havefunace.top

Ruby: u.is_a?(User)
来源：http://tqd.yj20258888.top

C#:   u is User
来源：http://zcb.shanyushiyangtech.top

[G14] 数据类 / record
来源：http://qwj.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cln.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://nog.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://qag.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://oso.bbcook.cn

Java: record User(String name, int age) {}
来源：http://nyq.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://xjs.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bmj.birdmap.top

C#:   record User(string Name, int Age);
来源：http://msf.cqqwz.cn

[G15] 枚举
来源：http://mgx.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sjr.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://xyi.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oym.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://erf.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://iwr.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lsu.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://end.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xdz.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://axo.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hwl.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://lor.fengsongda.top

JS:   Object.entries(obj)
来源：http://ooz.sxryk.cn

TS:   Object.entries(obj)
来源：http://xxd.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ihj.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dqz.sxryk.cn

Ruby: obj.instance_variables
来源：http://qco.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://ogl.ctjpmb.com

================================================================================
来源：http://jiy.birdmap.top

H. 异常与错误处理
来源：http://qtj.shuidangran.top

================================================================================
来源：http://sdm.316326.xyz

[H01] try / catch 基础
来源：http://rwn.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mbs.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aux.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ixg.chenlongwang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://viu.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ibq.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fex.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qsd.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gvh.yongpay.top

[H02] finally / ensure 收尾
来源：http://uvj.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://jmh.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lwl.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fhf.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jfh.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://adv.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rjb.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://odp.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mfz.ivvv.top

[H03] 主动抛出异常
来源：http://pol.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://kap.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gig.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://tzx.uphjek.com

TS:   throw new Error("错误信息");
来源：http://mzd.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://obt.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kpa.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gbn.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://zwg.cheryme.top

[H04] 自定义异常类型
来源：http://jzc.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://fwv.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cbu.fengsongda.top

JS:   class MyError extends Error {}
来源：http://epp.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://pbq.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://rrs.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hhl.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://upm.hcnkem.com

C#:   class MyException : Exception {}
来源：http://wns.nanxuanxn.top

[H05] 捕获特定类型
来源：http://gnu.svipenyu.cn

Py:   except ValueError as e:
来源：http://xzx.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ygp.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://bwl.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://kto.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://jfo.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nlr.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://pmh.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qan.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://oza.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://bew.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://qyl.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://cwv.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://gpc.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gkq.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bhg.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://owy.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://ntc.fzhhl.top

[H07] 断言
来源：http://cjr.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://lvv.gogol.net.cn

PHP:  assert($x > 0);
来源：http://ecj.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://egb.daria6918.cn

TS:   console.assert(x > 0);
来源：http://eua.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://tox.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://deu.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vbv.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://izw.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://fna.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://rkj.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nsx.guannengcc.top

JS:   e.message;  e.stack
来源：http://qtu.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dgl.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://voi.quarkkingdee.top

Go:   err.Error()
来源：http://phu.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://gig.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://wvy.fehbvm.com

[H09] 带错误码的异常
来源：http://gej.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mht.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hma.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wcq.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ggf.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yze.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ptm.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://wvw.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mgw.yuanzhike.top

[H10] 资源自动释放
来源：http://azc.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://iph.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ftw.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kgs.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fdh.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zzc.kuanghao11.cn

Go:   defer f.Close()
来源：http://jvt.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ihy.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lrx.pycfn.com

================================================================================
来源：http://iyw.jqgufenzy.top

I. 正则表达式
来源：http://wnt.yuanzhike.top

================================================================================
来源：http://snv.meibo888.top

[I01] 判断是否匹配
来源：http://rgf.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fum.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://exl.zycfv.cn

JS:   /\d+/.test(s)
来源：http://pqe.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://pqk.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://esf.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wew.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://dby.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xym.hesvh.cn

[I02] 提取所有匹配
来源：http://bse.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://cgz.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hix.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tvu.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://nib.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lvj.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zqf.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://tfv.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iuz.aizwys.cn

[I03] 提取捕获分组
来源：http://gcb.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xnx.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nbe.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zmt.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cwv.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yrz.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kpr.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ubd.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hbu.cashguo.top

[I04] 正则替换
来源：http://gmp.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xhz.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aoh.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uiz.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://dcz.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://jhl.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://luc.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kpg.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iqn.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://gsp.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ubr.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mmn.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://dkl.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://mgn.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://lcy.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pqg.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://khw.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://usi.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lof.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hys.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ehj.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mdt.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enb.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zip.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zpx.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jvg.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://roy.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://xkb.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bea.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qio.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bzs.daxiang520.top

TS:   /error/gim
来源：http://qmt.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tzf.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tyw.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://hhf.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cib.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://puw.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mhp.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dif.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vll.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkr.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nnd.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eip.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gbr.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mtp.zhixingplan.top

================================================================================
来源：http://ckr.ivvv.top

J. 日期与时间
来源：http://cwn.pengpengdd.cyou

================================================================================
来源：http://qyt.52xcode.cn

[J01] 获取当前时间
来源：http://stb.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ihc.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gog.hesvh.cn

JS:   new Date();  Date.now()
来源：http://ugj.aizwys.cn

TS:   new Date();  Date.now()
来源：http://zlq.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wdf.daxiang520.top

Go:   time.Now()
来源：http://dke.cheryme.top

Ruby: Time.now
来源：http://uvv.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://crp.xziqi.cn

[J02] 格式化输出
来源：http://jae.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cmf.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cgw.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sun.chenjidiqi.icu

TS:   d.toISOString()
来源：http://ngh.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oiv.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kjh.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fpi.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nus.yangfankeji.com

[J03] 字符串解析为日期
来源：http://unv.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://esu.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vwe.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://zjc.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://sxb.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://tvn.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zph.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://amj.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sai.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://mwh.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bgw.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yyg.hesvh.cn


<!-- 参考信息 -->