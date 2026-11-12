代发 wailian999

[G06] 重写方法
来源：http://ooz.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://rvi.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hqv.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://iad.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://wjj.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://nja.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://irs.yongpay.top

Ruby: def greet; "admin"; end
来源：http://xgw.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://bcy.yonumen.top

[G07] 调用父类方法
来源：http://ssi.zhoulong.xyz

Py:   super().greet()
来源：http://itq.cucudq.cn

PHP:  parent::greet();
来源：http://vzp.yongpay.top

JS:   super.greet();
来源：http://rkq.zhijiandao.cn

TS:   super.greet();
来源：http://ekd.xuetiantiany.cn

Java: super.greet();
来源：http://yod.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uvp.52xcode.cn

Ruby: super
来源：http://nuf.xylfe.cn

C#:   base.Greet();
来源：http://fzo.quarkkingdee.top

[G08] 静态方法与属性
来源：http://riq.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://orl.meibo888.top

PHP:  public static function f() {}
来源：http://ftw.zdqjudy.top

JS:   static f() {}
来源：http://efr.gaohongyu789.top

TS:   static f(): void {}
来源：http://wnu.jqgfzy.top

Java: static void f() {}
来源：http://dmm.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iml.xuetiantiany.cn

Ruby: def self.f; end
来源：http://twt.shanyushiyangkeji.top

C#:   public static void F() {}
来源：http://ien.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://nzh.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://huu.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yee.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://bxp.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://iht.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://qau.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://pef.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xqs.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://vwg.hnxiangtu.top

[G10] 访问控制
来源：http://hmh.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://wmq.tarul.cn

PHP:  public / protected / private
来源：http://muj.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://iiw.guowangkeji.top

TS:   public / protected / private
来源：http://qsj.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://rpg.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ziw.hnqzz.top

Ruby: public / protected / private
来源：http://tom.hywenlv.cn

C#:   public / protected / private / internal
来源：http://yjo.xuetiantiany.cn

[G11] getter / setter
来源：http://uqz.tanke756.top

Py:   @property 与 @x.setter
来源：http://zuq.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bgu.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://myd.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://lsj.ydzc1.top

Java: public String getName() { return name; }
来源：http://zay.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://akb.ppjwa.cn

Ruby: attr_accessor :name
来源：http://syx.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://euq.hnxiangtu.top

[G12] 对象转字符串
来源：http://ivm.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://kug.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://joa.cucudq.cn

JS:   toString() { return this.name; }
来源：http://paq.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://bxo.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://azo.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sii.andypj.xyz

Ruby: def to_s; @name; end
来源：http://qkd.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://jbb.ydjk.org.cn

[G13] 判断对象类型
来源：http://gwe.0kj1m.cn

Py:   isinstance(u, User)
来源：http://qwl.sjlbkw.cn

PHP:  $u instanceof User
来源：http://clg.shuidangran.top

JS:   u instanceof User
来源：http://vkh.yuanzhike.top

TS:   u instanceof User
来源：http://dgv.ywan-chungtsiang.top

Java: u instanceof User
来源：http://fnw.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://seu.cucudq.cn

Ruby: u.is_a?(User)
来源：http://xdm.guowangkeji.top

C#:   u is User
来源：http://gho.jinqigfzy.top

[G14] 数据类 / record
来源：http://swu.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ndu.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://rel.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://apv.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://ahl.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://vmg.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://enm.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hbn.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://lon.ydzc1.top

[G15] 枚举
来源：http://yts.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ivi.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://asc.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://elm.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kos.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://wpo.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qsq.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://ggw.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://muc.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://hcp.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fce.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://pbl.iojbl.cn

JS:   Object.entries(obj)
来源：http://wep.hysaishi.cn

TS:   Object.entries(obj)
来源：http://opq.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gvo.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://auk.pycfn.com

Ruby: obj.instance_variables
来源：http://mqa.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://uei.fanxiaobao.xyz

================================================================================
来源：http://xrc.andypj.xyz

H. 异常与错误处理
来源：http://ssp.haohaochexian.top

================================================================================
来源：http://maj.cheryme.top

[H01] try / catch 基础
来源：http://dph.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cxy.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uah.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xmt.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zyw.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pnt.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://srx.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xmn.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xor.hcnkem.com

[H02] finally / ensure 收尾
来源：http://gzy.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://uqa.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mvh.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nia.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nzj.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bbx.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rxx.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gti.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gkl.yonumen.top

[H03] 主动抛出异常
来源：http://gdi.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://fgg.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iak.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://cyn.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://szi.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kzt.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xem.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wpe.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ybm.xingfuxueyuan.xyz

[H04] 自定义异常类型
来源：http://amv.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://iui.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://fqs.nwbrower.top

JS:   class MyError extends Error {}
来源：http://cue.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://aqq.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://jlw.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajz.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://fhz.yvedp.cn

C#:   class MyException : Exception {}
来源：http://ple.yongpay.top

[H05] 捕获特定类型
来源：http://jok.zdbjq.cn

Py:   except ValueError as e:
来源：http://fyx.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hlp.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://wiv.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://why.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://yrq.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vlj.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://jsx.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mry.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://ysw.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://kkb.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://ckd.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://bus.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://nxn.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gkf.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xoe.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://zsd.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://why.snrcjt.cn

[H07] 断言
来源：http://qmr.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://igw.daxiang520.top

PHP:  assert($x > 0);
来源：http://hqh.yueranfly.top

JS:   console.assert(x > 0);
来源：http://aph.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://mut.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://mes.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgy.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://tsr.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://ifn.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://fxj.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://jln.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qxt.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://ufm.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://plf.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vek.cdnleiting.top

Go:   err.Error()
来源：http://efm.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://sdc.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://woo.cucudq.cn

[H09] 带错误码的异常
来源：http://ksc.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cfo.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nie.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oqn.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gju.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ufp.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xoa.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ovg.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xyc.xuetiantiany.cn

[H10] 资源自动释放
来源：http://rvu.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tpw.tarul.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://afm.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vjb.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bvy.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jkc.jianghu66.top

Go:   defer f.Close()
来源：http://eeb.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zpq.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eaw.guannengcc.top

================================================================================
来源：http://ims.jqgfzy.top

I. 正则表达式
来源：http://dsi.gogol.net.cn

================================================================================
来源：http://iqg.xinyue.icu

[I01] 判断是否匹配
来源：http://jjv.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rel.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pxl.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://btx.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://rqh.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fvd.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wtq.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://lij.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mdn.ctjpmb.com

[I02] 提取所有匹配
来源：http://ygd.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://osr.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iet.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iqs.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://fyj.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xbb.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gcl.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://qgr.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbv.uphjek.com

[I03] 提取捕获分组
来源：http://rfg.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://apf.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://srn.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xmi.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ldh.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qtl.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://put.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xzt.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eso.aizwys.cn

[I04] 正则替换
来源：http://hgk.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jub.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ypb.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lxs.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://dof.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://zwq.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yfo.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://pqk.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ang.zhengqikj.top

[I05] 按正则拆分
来源：http://dod.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mks.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wwr.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://nzi.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://tqq.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://uks.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ozc.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bto.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tmg.havefunace.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xpp.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ynu.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://onm.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kgg.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wqa.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://udy.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://weu.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tma.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bkl.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://zah.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zsw.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wwg.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ppf.zdqjudy.top

TS:   /error/gim
来源：http://qgq.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lkz.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dfk.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://qtt.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://njt.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://nfn.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pai.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ypk.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cwx.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://amz.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://ldc.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iki.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://joq.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vau.nanxinkj.top

================================================================================
来源：http://oaq.dianchejie.cn

J. 日期与时间
来源：http://mmq.andypj.xyz

================================================================================
来源：http://lww.zdbjq.cn

[J01] 获取当前时间
来源：http://fuk.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bry.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xtd.yj202588.top

JS:   new Date();  Date.now()
来源：http://dkz.cucudq.cn

TS:   new Date();  Date.now()
来源：http://ybk.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jms.9152youxi.cn

Go:   time.Now()
来源：http://tqr.cashguo.top

Ruby: Time.now
来源：http://cvf.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wfs.tarul.cn

[J02] 格式化输出
来源：http://lwh.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rkp.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jfj.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://idm.tianlin.xyz

TS:   d.toISOString()
来源：http://mlu.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tag.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://emm.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mrb.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zwi.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://boj.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wgp.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ppq.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://isv.birdmap.top

TS:   new Date("2024-01-02")
来源：http://xhe.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gmj.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://srt.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://tsi.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nyy.vehdjk.com

[J04] 时间戳与日期互转
来源：http://eqn.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wgk.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yqw.sweek.top


<!-- 参考信息 -->