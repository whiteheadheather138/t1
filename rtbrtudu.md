代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://aag.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://ebv.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://loh.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://ilj.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://kxc.52xcode.cn

[G07] 调用父类方法
来源：http://duc.ivvv.top

Py:   super().greet()
来源：http://pjk.daria6918.cn

PHP:  parent::greet();
来源：http://jlb.chenzaomai.com

JS:   super.greet();
来源：http://vzh.ybcxt.top

TS:   super.greet();
来源：http://guq.tian-w.cn

Java: super.greet();
来源：http://usx.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://klc.epnwcf.com

Ruby: super
来源：http://uzs.quarkkingdee.top

C#:   base.Greet();
来源：http://hwr.mhx1999.top

[G08] 静态方法与属性
来源：http://kgo.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kmb.zhoulong.xyz

PHP:  public static function f() {}
来源：http://rtz.guannengcc.top

JS:   static f() {}
来源：http://jfh.redwolf501.top

TS:   static f(): void {}
来源：http://yrt.epnwcf.com

Java: static void f() {}
来源：http://tul.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://dpv.tarul.cn

Ruby: def self.f; end
来源：http://yiq.sweek.top

C#:   public static void F() {}
来源：http://ohq.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://yuk.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://gal.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://btx.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lvg.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://adz.daria6918.cn

Java: interface Shape { double area(); }
来源：http://yzd.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://skv.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gxc.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://clk.zhiwuduotai.top

[G10] 访问控制
来源：http://gum.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://szw.quarkkingdee.top

PHP:  public / protected / private
来源：http://grd.bbcook.cn

JS:   #private 字段；其余公开
来源：http://piv.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://aph.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://qps.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://awg.chenzaomai.com

Ruby: public / protected / private
来源：http://fqx.316326.xyz

C#:   public / protected / private / internal
来源：http://wln.yvedp.cn

[G11] getter / setter
来源：http://hzw.hcnkem.com

Py:   @property 与 @x.setter
来源：http://myj.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jcn.tarul.cn

JS:   get name() { return this._name; }
来源：http://qnw.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://dfk.yueranfly.top

Java: public String getName() { return name; }
来源：http://xgq.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://igs.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://qki.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://rvh.shuidangran.top

[G12] 对象转字符串
来源：http://wfc.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://yku.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://upu.xziqi.cn

JS:   toString() { return this.name; }
来源：http://nbb.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://ols.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://epg.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://rgc.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://jkj.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://szv.andypj.xyz

[G13] 判断对象类型
来源：http://ghp.zhengqikj.top

Py:   isinstance(u, User)
来源：http://lbv.aizwys.cn

PHP:  $u instanceof User
来源：http://ktr.nanxuanxn.top

JS:   u instanceof User
来源：http://xda.ehwqpu.com

TS:   u instanceof User
来源：http://qms.kuanghao11.cn

Java: u instanceof User
来源：http://xhv.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nep.meibo888.top

Ruby: u.is_a?(User)
来源：http://cgs.gogol.net.cn

C#:   u is User
来源：http://ptb.aibaodan.cn

[G14] 数据类 / record
来源：http://rnx.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://alq.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://nnt.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wjy.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://sgm.guannengcc.top

Java: record User(String name, int age) {}
来源：http://ebd.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://mwj.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fej.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://jsw.hammf.cn

[G15] 枚举
来源：http://uuq.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rtu.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sbs.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://quk.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dis.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://rnz.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qqo.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://lqb.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zsm.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://ozi.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jvr.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://kit.hywenlv.cn

JS:   Object.entries(obj)
来源：http://jxe.yj20258888.top

TS:   Object.entries(obj)
来源：http://obh.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://psr.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gbi.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://eao.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://gza.pengpengdd.cyou

================================================================================
来源：http://lew.gzhubu.top

H. 异常与错误处理
来源：http://khk.nanxuanxn.top

================================================================================
来源：http://bqy.dianchejie.cn

[H01] try / catch 基础
来源：http://zhn.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yll.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qms.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://axn.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gbs.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nir.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tjt.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://skj.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qcj.xylfe.cn

[H02] finally / ensure 收尾
来源：http://xbg.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iao.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://grh.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://klh.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fit.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://ths.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jtx.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xkz.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://avc.cheryme.top

[H03] 主动抛出异常
来源：http://dbz.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://nps.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rix.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://tge.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://jvo.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://pid.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xvx.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://exp.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://tex.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://trl.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://tuv.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://cxi.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://crp.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://nvd.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://lpb.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://awi.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://sox.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://jid.316326.xyz

[H05] 捕获特定类型
来源：http://rmp.jyoumei.cn

Py:   except ValueError as e:
来源：http://zpu.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ymv.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://tfa.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://oah.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://jjs.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gwj.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://xhg.sxryk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rlm.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://wwt.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://ymz.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bax.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://nzb.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zbc.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qlc.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xno.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://stg.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://vap.shanyushiyangkeji.top

[H07] 断言
来源：http://ntb.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://ecs.jqgfzy.top

PHP:  assert($x > 0);
来源：http://vul.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://tkt.yj20258888.top

TS:   console.assert(x > 0);
来源：http://qay.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://bql.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oqz.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://aqe.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://icy.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://oaa.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://hmi.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zcc.guannengcc.top

JS:   e.message;  e.stack
来源：http://gur.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://brr.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nmq.dianchejie.cn

Go:   err.Error()
来源：http://zuv.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://mml.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://kgj.hesvh.cn

[H09] 带错误码的异常
来源：http://zzh.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vxd.yj20258888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eth.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vyu.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tfj.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://poh.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hug.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://nqz.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ifc.hnxiangtu.top

[H10] 资源自动释放
来源：http://jag.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://avv.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xyr.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://enc.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cfa.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yxx.kuanghao11.cn

Go:   defer f.Close()
来源：http://tef.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ina.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wvp.sjlbkw.cn

================================================================================
来源：http://wdb.sufxvd.cn

I. 正则表达式
来源：http://qfr.tarul.cn

================================================================================
来源：http://jif.hysaishi.cn

[I01] 判断是否匹配
来源：http://htq.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xna.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vos.cashguo.top

JS:   /\d+/.test(s)
来源：http://wqi.daria6918.cn

TS:   /\d+/.test(s)
来源：http://pgm.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jph.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jvy.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://wla.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zsm.sjlbkw.cn

[I02] 提取所有匹配
来源：http://wea.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://nmg.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vhi.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zpf.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://sft.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hji.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uto.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://nll.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ttu.chenlongwang.top

[I03] 提取捕获分组
来源：http://esf.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sqw.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pkb.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fec.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://itj.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ene.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lhf.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cla.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lmq.zhongyouzk.top

[I04] 正则替换
来源：http://jvz.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fni.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wnl.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://xdv.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jgf.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://ndt.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zay.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nnj.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://beh.hcnkem.com

[I05] 按正则拆分
来源：http://mbh.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qcu.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bdu.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://how.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://men.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://rtu.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rny.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://lnk.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xbf.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wot.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dnr.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mnp.ydzc1.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ciq.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pxm.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ikl.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://knh.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fod.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mfi.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://eim.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wbs.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qhk.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://epo.daxiang520.top

TS:   /error/gim
来源：http://esm.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gez.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yhh.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://vyd.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://skg.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://tuv.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hnn.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zhl.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qec.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hhs.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://zje.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kkv.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://chk.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mmr.zhijiandao.cn

================================================================================
来源：http://fko.dianchejie.cn

J. 日期与时间
来源：http://lqt.wangdashe.top

================================================================================
来源：http://jdp.hesvh.cn

[J01] 获取当前时间
来源：http://cxa.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lsa.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hbl.yj20258888.top

JS:   new Date();  Date.now()
来源：http://ruk.uphjek.com

TS:   new Date();  Date.now()
来源：http://obr.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vdh.cucudq.cn

Go:   time.Now()
来源：http://vhq.xinyue.icu

Ruby: Time.now
来源：http://yux.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rye.ehwqpu.com

[J02] 格式化输出
来源：http://hni.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gas.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zeu.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://njp.sjlbkw.cn

TS:   d.toISOString()
来源：http://uhv.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ikh.zdqjudy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ecf.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://koi.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lpj.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://ocf.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rtr.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sjh.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://ysg.meibo888.top

TS:   new Date("2024-01-02")
来源：http://tzx.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://shp.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uew.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ieg.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jdb.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://tgk.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eaw.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xma.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ume.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://hcf.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://njh.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://whv.ydzc1.top


<!-- 参考信息 -->