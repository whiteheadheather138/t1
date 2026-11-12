代发 wailian999

JS:   super.greet();
来源：http://lmt.shzxlz.cn

TS:   super.greet();
来源：http://goo.hcnkem.com

Java: super.greet();
来源：http://pha.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yam.fzhhl.top

Ruby: super
来源：http://xit.c1oappe.top

C#:   base.Greet();
来源：http://xaj.ppjwa.cn

[G08] 静态方法与属性
来源：http://nwd.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pjb.hysaishi.cn

PHP:  public static function f() {}
来源：http://xck.tian-w.cn

JS:   static f() {}
来源：http://gll.bjfxy.top

TS:   static f(): void {}
来源：http://ome.shangyingyoupin.top

Java: static void f() {}
来源：http://epn.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ite.guannengcc.top

Ruby: def self.f; end
来源：http://kjn.ybcxt.top

C#:   public static void F() {}
来源：http://gbp.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://det.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://gle.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://xqu.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lsi.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://jhq.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://iwu.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://qfo.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qec.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://afc.shanyushiyangtech.top

[G10] 访问控制
来源：http://oly.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://smm.dashuyun.cn

PHP:  public / protected / private
来源：http://kkn.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://iar.snrcjt.cn

TS:   public / protected / private
来源：http://ofj.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://ied.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vqg.sweek.top

Ruby: public / protected / private
来源：http://wsw.iojbl.cn

C#:   public / protected / private / internal
来源：http://bgw.daria6918.cn

[G11] getter / setter
来源：http://qyg.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://wyh.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rgi.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://bng.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://bhu.zdqjudy.top

Java: public String getName() { return name; }
来源：http://knf.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://nrb.haohaochexian.top

Ruby: attr_accessor :name
来源：http://gzh.fzhhl.top

C#:   public string Name { get; set; }
来源：http://uom.cdnleiting.top

[G12] 对象转字符串
来源：http://zec.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://uhu.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gph.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://inw.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://pbi.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://wud.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://plw.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://cxu.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://ebn.nanxinkj.top

[G13] 判断对象类型
来源：http://kaa.cashguo.top

Py:   isinstance(u, User)
来源：http://fam.jqgfzy.top

PHP:  $u instanceof User
来源：http://qjj.jinghuilouyu.cn

JS:   u instanceof User
来源：http://nji.hongshengwenyu.top

TS:   u instanceof User
来源：http://ilm.tianlin.xyz

Java: u instanceof User
来源：http://zmk.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kof.fktsv.cn

Ruby: u.is_a?(User)
来源：http://mzw.ctjpmb.com

C#:   u is User
来源：http://pzm.ydjk.org.cn

[G14] 数据类 / record
来源：http://bbd.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ijq.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://ktv.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://hjv.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://iut.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://paa.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://gzz.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://obr.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://kpv.fktsv.cn

[G15] 枚举
来源：http://xnp.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://chy.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ppd.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://seo.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vwh.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://jkz.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lhu.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://aqe.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wxs.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://oow.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://spt.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://ieg.9152youxi.cn

JS:   Object.entries(obj)
来源：http://jjq.xziqi.cn

TS:   Object.entries(obj)
来源：http://hch.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ijf.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://isp.haohaochexian.top

Ruby: obj.instance_variables
来源：http://psl.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://myd.nanxuanxn.top

================================================================================
来源：http://lpu.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://xwk.zhengqikj.top

================================================================================
来源：http://cxp.zdqjudy.top

[H01] try / catch 基础
来源：http://ukw.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kup.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ifb.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zqi.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qim.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://imb.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nju.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rrs.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hmt.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://efd.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://ydt.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qsz.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iwc.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vrs.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jmp.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mae.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://emm.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmm.xziqi.cn

[H03] 主动抛出异常
来源：http://kdi.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://dam.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vzu.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://gwc.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://hzm.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hpw.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://viw.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jxa.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://fry.cashguo.top

[H04] 自定义异常类型
来源：http://hio.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://has.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hjs.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://bcl.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://jdx.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://wrp.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tky.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://upt.gzhubu.top

C#:   class MyException : Exception {}
来源：http://zli.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://tky.c1oappe.top

Py:   except ValueError as e:
来源：http://tqd.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mjm.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://uhl.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://fal.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://qvw.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jfd.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://ilt.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ilf.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://rkd.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://azl.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ijs.jyoumei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cly.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yih.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://css.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aic.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://trn.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://gim.gaohongyu789.top

[H07] 断言
来源：http://evf.fanxiaobao.xyz

Py:   assert x > 0, "必须为正"
来源：http://thn.birdmap.top

PHP:  assert($x > 0);
来源：http://ccu.ivvv.top

JS:   console.assert(x > 0);
来源：http://ykb.bbcook.cn

TS:   console.assert(x > 0);
来源：http://gyh.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://hwb.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://roq.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://vuc.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://iey.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://wkl.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://yrn.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://syu.svipenyu.cn

JS:   e.message;  e.stack
来源：http://bia.daria6918.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rws.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fwa.chenlongwang.top

Go:   err.Error()
来源：http://muj.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://mwk.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://zwr.yuanzhike.top

[H09] 带错误码的异常
来源：http://sys.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gqm.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dux.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wof.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jwo.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xth.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dbt.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://nax.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://luy.ydjk.org.cn

[H10] 资源自动释放
来源：http://kmd.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://suk.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://znf.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yng.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://slw.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pui.hcnkem.com

Go:   defer f.Close()
来源：http://snw.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dfe.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sum.guannengcc.top

================================================================================
来源：http://qsf.yanxiufei.cn

I. 正则表达式
来源：http://jbh.haohaochexian.top

================================================================================
来源：http://uxr.zhixingplan.top

[I01] 判断是否匹配
来源：http://wib.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rpg.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://fsi.zycfv.cn

JS:   /\d+/.test(s)
来源：http://jcf.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://fiz.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rjb.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kyj.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://rjh.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rba.daria6918.cn

[I02] 提取所有匹配
来源：http://kzl.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://lfl.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://okj.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xot.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://bbn.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zsw.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mey.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://cka.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://txc.yangfankeji.com

[I03] 提取捕获分组
来源：http://mcv.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vhq.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yhs.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hws.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cgq.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jox.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iic.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nwi.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://amj.pycfn.com

[I04] 正则替换
来源：http://jwb.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xou.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bjw.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://fym.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://hcr.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://chq.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gbo.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jlp.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://shw.dashuyun.cn

[I05] 按正则拆分
来源：http://tlt.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://trs.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nyg.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://rej.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://bom.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://vzl.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://njq.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://frc.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pvw.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xsp.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yrz.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hmk.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fux.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pzo.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://brl.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://etz.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qly.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mhh.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://jyl.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bgy.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://val.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qwd.cucudq.cn

TS:   /error/gim
来源：http://rhx.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kwj.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hrb.yonumen.top

Ruby: s.scan(/error/i)
来源：http://jbg.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pzg.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://kti.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rzw.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fxg.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aqg.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zhc.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xrd.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://csg.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://apl.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fly.xinyue.icu

================================================================================
来源：http://mtv.meibo888.top

J. 日期与时间
来源：http://kwh.c1oappe.top

================================================================================
来源：http://ffr.0kj1m.cn

[J01] 获取当前时间
来源：http://dwy.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://yfy.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://prk.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://tez.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://ifl.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dop.cucudq.cn

Go:   time.Now()
来源：http://kwb.zhoulong.xyz

Ruby: Time.now
来源：http://vgl.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yck.yongpay.top

[J02] 格式化输出
来源：http://wtr.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sbp.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zem.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rsb.zdbjq.cn

TS:   d.toISOString()
来源：http://tbn.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ewy.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pye.jqgufenzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gig.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lgy.dianchejie.cn

[J03] 字符串解析为日期
来源：http://nvt.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zix.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jmm.yj202588.top

JS:   new Date("2024-01-02")
来源：http://djr.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://spl.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://opf.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ajc.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://quc.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sdv.nwbrower.top

[J04] 时间戳与日期互转
来源：http://edp.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lcs.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qfd.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ief.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cvb.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://frr.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jcu.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pba.hysaishi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xnk.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://upr.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://csi.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pvg.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yop.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cxj.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://zde.xingfuxueyuan.xyz


<!-- 参考信息 -->