代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://gjv.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://abc.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://top.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://ohx.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://wkz.fehbvm.com

[G07] 调用父类方法
来源：http://dca.ybcxt.top

Py:   super().greet()
来源：http://fxs.ydzc1.top

PHP:  parent::greet();
来源：http://fyy.fanxiaobao.xyz

JS:   super.greet();
来源：http://qek.shanyushiyangkeji.top

TS:   super.greet();
来源：http://efx.yj20258888.top

Java: super.greet();
来源：http://zxe.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://elh.fanxiaobao.xyz

Ruby: super
来源：http://use.gogol.net.cn

C#:   base.Greet();
来源：http://mmc.nwbrower.top

[G08] 静态方法与属性
来源：http://sgo.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fxb.yueranfly.top

PHP:  public static function f() {}
来源：http://qol.daria6918.cn

JS:   static f() {}
来源：http://vec.aibaodan.cn

TS:   static f(): void {}
来源：http://sqg.daria6918.cn

Java: static void f() {}
来源：http://gru.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://keu.jianghu66.top

Ruby: def self.f; end
来源：http://kkr.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://oly.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://dxx.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://tuf.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://avj.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pgt.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://lym.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://kvv.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://fet.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://roo.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://vkb.cucudq.cn

[G10] 访问控制
来源：http://pxn.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://bpv.nwbrower.top

PHP:  public / protected / private
来源：http://ufs.cucudq.cn

JS:   #private 字段；其余公开
来源：http://abm.yonumen.top

TS:   public / protected / private
来源：http://epl.316326.xyz

Java: public / protected / private / 默认包级
来源：http://bxt.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ast.guannengcc.top

Ruby: public / protected / private
来源：http://mpn.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://tns.mhx1999.top

[G11] getter / setter
来源：http://qlk.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://eda.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://hmc.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://wrb.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://wkf.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://paq.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://eoy.bbcook.cn

Ruby: attr_accessor :name
来源：http://ziy.birdmap.top

C#:   public string Name { get; set; }
来源：http://yip.yj202588.top

[G12] 对象转字符串
来源：http://khj.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://xxl.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xvz.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://whc.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://pjo.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://dtp.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xpp.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://whi.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://fuv.quarkkingdee.top

[G13] 判断对象类型
来源：http://ohs.yonumen.top

Py:   isinstance(u, User)
来源：http://xhp.shzxlz.cn

PHP:  $u instanceof User
来源：http://fpv.cheryme.top

JS:   u instanceof User
来源：http://xna.hnxiangtu.top

TS:   u instanceof User
来源：http://ulx.vehdjk.com

Java: u instanceof User
来源：http://pwq.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vfh.bjfxy.top

Ruby: u.is_a?(User)
来源：http://fpd.shanyushiyangkeji.top

C#:   u is User
来源：http://irq.shuidangran.top

[G14] 数据类 / record
来源：http://qyf.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zha.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://eap.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tby.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://uts.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://lgz.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://zqp.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hkr.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://awi.zdqjudy.top

[G15] 枚举
来源：http://fbb.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tjq.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tgh.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nng.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mqf.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://wvi.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jxx.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://agy.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://val.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://nrx.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xeq.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://evg.guowangkeji.top

JS:   Object.entries(obj)
来源：http://tfm.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://pxq.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ldn.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://swk.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://zti.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://aoc.yuanzhike.top

================================================================================
来源：http://tcf.chenlongwang.top

H. 异常与错误处理
来源：http://tgx.hysaishi.cn

================================================================================
来源：http://plv.jlsjyb.cn

[H01] try / catch 基础
来源：http://glr.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://etr.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tml.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://asj.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tks.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://efb.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://art.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lgy.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eey.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://eod.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://bab.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uhe.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jzt.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://gno.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://tlx.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ysn.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xxc.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://orl.daxiang520.top

[H03] 主动抛出异常
来源：http://bza.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://mxn.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ksc.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://qoz.yj20258.top

TS:   throw new Error("错误信息");
来源：http://vnx.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://per.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pqt.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://mav.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://wmr.yj20258888.top

[H04] 自定义异常类型
来源：http://zob.birdmap.top

Py:   class MyError(Exception): pass
来源：http://qyi.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://cbi.aizwys.cn

JS:   class MyError extends Error {}
来源：http://mfp.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://qpm.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://yiy.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oai.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://hmr.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://ubm.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://vxq.snrcjt.cn

Py:   except ValueError as e:
来源：http://wms.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rfi.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://mvv.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://xev.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://kbg.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hql.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://nqv.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dhy.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://yqb.bjfxy.top

Py:   value = d.get("k") or default
来源：http://eao.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://tja.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fwb.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ruj.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lda.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://raz.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://jhq.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://ksm.fehbvm.com

[H07] 断言
来源：http://hrh.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://xei.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://euz.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://pgg.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://utf.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://cdd.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fkh.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zql.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://bkt.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://bza.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://tue.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yiy.aizwys.cn

JS:   e.message;  e.stack
来源：http://siq.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://him.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://set.iojbl.cn

Go:   err.Error()
来源：http://fsk.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://cgw.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://est.tian-w.cn

[H09] 带错误码的异常
来源：http://mbx.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tvi.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jvj.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ogp.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jht.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ped.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vpj.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://lvu.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://siz.shzxlz.cn

[H10] 资源自动释放
来源：http://erv.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://qkg.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eeo.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wmx.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dug.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ybs.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://qmz.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fxz.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://feo.zhiwuduotai.top

================================================================================
来源：http://jwt.jqgfzy.top

I. 正则表达式
来源：http://ydw.9152youxi.cn

================================================================================
来源：http://wbd.havefunace.top

[I01] 判断是否匹配
来源：http://rvy.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vhb.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ydo.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://hqe.tanke756.top

TS:   /\d+/.test(s)
来源：http://uxx.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kjv.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kqy.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://tpv.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pwy.bjfxy.top

[I02] 提取所有匹配
来源：http://edd.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://ytg.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cvu.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bwf.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://own.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ene.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ojk.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://sgd.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zrk.zdqjudy.top

[I03] 提取捕获分组
来源：http://ymd.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://boi.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gyq.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jga.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lhy.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cpx.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xpb.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bhf.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://occ.52xcode.cn

[I04] 正则替换
来源：http://qlj.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://evu.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ttq.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pie.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://pll.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vvk.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://auf.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ttc.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://epm.ehwqpu.com

[I05] 按正则拆分
来源：http://sdc.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eur.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cvn.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://rkc.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://cwq.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://xlp.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ejd.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://far.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sht.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wlk.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xtn.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yba.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mwp.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vnv.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nww.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rma.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pqz.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pqa.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://toa.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gjs.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ybk.daria6918.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dcn.haohaochexian.top

TS:   /error/gim
来源：http://sel.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tbq.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cyc.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://nhk.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mhx.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://qxj.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sxq.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wio.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kid.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wbf.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://jlp.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rag.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://djm.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fsk.nanxuanxn.top

================================================================================
来源：http://wzb.yuxming.cn

J. 日期与时间
来源：http://elr.yuanzhike.top

================================================================================
来源：http://fyz.feifeiyinyue.top

[J01] 获取当前时间
来源：http://whv.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oul.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fmu.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://ksb.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://tzn.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://tii.guowangkeji.top

Go:   time.Now()
来源：http://goq.shangyingyoupin.top

Ruby: Time.now
来源：http://qkp.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cne.cashguo.top

[J02] 格式化输出
来源：http://iwe.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hlp.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sab.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hbk.52xcode.cn

TS:   d.toISOString()
来源：http://chx.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tmh.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iuk.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzz.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vep.uphjek.com

[J03] 字符串解析为日期
来源：http://vlr.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://krm.vehdjk.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cvi.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://rmk.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://hex.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zhf.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://udm.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://cer.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gjk.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://byt.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://acm.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vvb.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kyv.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://urv.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rbi.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dji.feifeiyinyue.top


<!-- 参考信息 -->