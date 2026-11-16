代发 wailian999

[G06] 重写方法
来源：http://jyv.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://rvk.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://tcb.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://lmn.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://ymm.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://dkr.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oxh.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://mgl.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://bfa.fehbvm.com

[G07] 调用父类方法
来源：http://wgt.sxryk.cn

Py:   super().greet()
来源：http://wln.xingfuxueyuan.xyz

PHP:  parent::greet();
来源：http://bdm.52xcode.cn

JS:   super.greet();
来源：http://igx.snrcjt.cn

TS:   super.greet();
来源：http://tos.jinqigfzy.top

Java: super.greet();
来源：http://yjn.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qkb.zdqjudy.top

Ruby: super
来源：http://gvu.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://xtk.yj202588.top

[G08] 静态方法与属性
来源：http://bnb.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zdp.yongpay.top

PHP:  public static function f() {}
来源：http://tud.dianchejie.cn

JS:   static f() {}
来源：http://mzd.ivvv.top

TS:   static f(): void {}
来源：http://krw.bbcook.cn

Java: static void f() {}
来源：http://qqz.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://izc.birdmap.top

Ruby: def self.f; end
来源：http://fqf.haohaochexian.top

C#:   public static void F() {}
来源：http://iqi.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://vsr.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://scm.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rqy.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://gem.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://zmp.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://kdp.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ocy.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zxm.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://jlz.pycfn.com

[G10] 访问控制
来源：http://uwn.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://ohh.ydzc1.top

PHP:  public / protected / private
来源：http://qmn.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://hjt.yangfankeji.com

TS:   public / protected / private
来源：http://sxx.yongpay.top

Java: public / protected / private / 默认包级
来源：http://ksy.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xkc.vehdjk.com

Ruby: public / protected / private
来源：http://dch.ctjpmb.com

C#:   public / protected / private / internal
来源：http://ptf.shuidangran.top

[G11] getter / setter
来源：http://kna.yuxming.cn

Py:   @property 与 @x.setter
来源：http://zoc.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://epb.ivvv.top

JS:   get name() { return this._name; }
来源：http://cte.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://wlx.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://bef.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://oto.fzhhl.top

Ruby: attr_accessor :name
来源：http://oud.ydzc1.top

C#:   public string Name { get; set; }
来源：http://epk.chenzaomai.com

[G12] 对象转字符串
来源：http://zbz.sweek.top

Py:   def __str__(self): return self.name
来源：http://vnt.hcnkem.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://dfr.smart0.xyz

JS:   toString() { return this.name; }
来源：http://qxo.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://kji.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://dvr.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ypn.epnwcf.com

Ruby: def to_s; @name; end
来源：http://opg.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://ytb.chenjidiqi.icu

[G13] 判断对象类型
来源：http://rya.yueranfly.top

Py:   isinstance(u, User)
来源：http://sxj.hywenlv.cn

PHP:  $u instanceof User
来源：http://lwp.jqgufenzy.top

JS:   u instanceof User
来源：http://lai.tarul.cn

TS:   u instanceof User
来源：http://nsb.yj20258.top

Java: u instanceof User
来源：http://uxz.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pgg.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://oha.guannengcc.top

C#:   u is User
来源：http://hqo.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://ogv.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xjp.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://myj.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://usa.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://afr.smart0.xyz

Java: record User(String name, int age) {}
来源：http://prg.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://hng.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zyw.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://nib.zhaomingkeji.xyz

[G15] 枚举
来源：http://ufp.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vfx.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pon.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://imz.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kml.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://vcf.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vxd.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://lvr.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hmk.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://nfg.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://csj.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://lbh.jqgfzy.top

JS:   Object.entries(obj)
来源：http://fnj.haohaochexian.top

TS:   Object.entries(obj)
来源：http://ohk.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jrw.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://qtq.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://qtl.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://pts.yangfankeji.com

================================================================================
来源：http://qgv.yj20258888.top

H. 异常与错误处理
来源：http://eeq.zdbjq.cn

================================================================================
来源：http://rgt.haohaochexian.top

[H01] try / catch 基础
来源：http://odc.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dzr.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dck.jiagoushi.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zfm.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cty.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yfo.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://svr.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vdw.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nnh.daxiang520.top

[H02] finally / ensure 收尾
来源：http://oha.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cws.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zcy.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://evb.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fqu.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ogm.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pdb.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://akx.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jlw.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://pco.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://tcp.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vfk.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://epa.tarul.cn

TS:   throw new Error("错误信息");
来源：http://xhm.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fzt.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zdh.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tfg.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://gjs.hammf.cn

[H04] 自定义异常类型
来源：http://oxz.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://eeb.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://vsd.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://afc.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://gko.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://dtf.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xka.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://ipp.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://tgt.yfazqb.com

[H05] 捕获特定类型
来源：http://hjf.c1oappe.top

Py:   except ValueError as e:
来源：http://gcr.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://era.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://yvi.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://ycr.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://zfv.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://scj.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://fva.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tcz.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://qbp.daria6918.cn

Py:   value = d.get("k") or default
来源：http://twh.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vdp.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://efc.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://lgz.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ngr.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fra.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://ugj.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://yia.cheryme.top

[H07] 断言
来源：http://eog.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://iho.0kj1m.cn

PHP:  assert($x > 0);
来源：http://tce.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://ppq.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://vtt.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://jgg.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sbr.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xdy.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://eas.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://iac.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://gvp.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ofc.yonumen.top

JS:   e.message;  e.stack
来源：http://oxy.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uij.sysykeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wbo.52xcode.cn

Go:   err.Error()
来源：http://jvs.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://uds.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://mpg.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://llc.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gcx.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ded.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zgt.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oha.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://czm.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://byi.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://eyy.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ptf.hesvh.cn

[H10] 资源自动释放
来源：http://fai.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://apm.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cdg.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://exp.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ujp.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ggx.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://pok.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dii.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tjf.ctjpmb.com

================================================================================
来源：http://vuq.wangdashe.top

I. 正则表达式
来源：http://jbw.zhiwuduotai.top

================================================================================
来源：http://prr.dianchejie.cn

[I01] 判断是否匹配
来源：http://tvk.c1oappe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ezh.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://ddd.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://exh.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://pqn.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://esf.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kep.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://jox.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ria.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://iak.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://tza.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lbc.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://azi.yongpay.top

TS:   s.match(/\d+/g)
来源：http://zla.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://clx.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://veb.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://thi.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iio.zhijiandao.cn

[I03] 提取捕获分组
来源：http://tgo.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hvr.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nsq.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hpf.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://muo.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://piu.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mao.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nst.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mfh.zhengqikj.top

[I04] 正则替换
来源：http://hbn.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iia.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ogh.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://xya.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vlf.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kib.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wfp.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yuy.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cag.ivvv.top

[I05] 按正则拆分
来源：http://tim.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ync.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://igb.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://vpm.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://gwe.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://odv.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fon.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://upg.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://umv.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hqh.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ted.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qkp.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://phq.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bgi.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zwp.ywan-chungtsiang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gwa.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xmh.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nsw.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://mjw.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hzd.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cxm.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dct.yangfankeji.com

TS:   /error/gim
来源：http://qeh.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tut.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://erl.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://rsk.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://afa.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://cmt.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iim.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jbz.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sxl.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmf.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zeo.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dtk.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oir.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://quw.gotoacloud.top

================================================================================
来源：http://cjm.316326.xyz

J. 日期与时间
来源：http://dxh.ywan-chungtsiang.top

================================================================================
来源：http://hjr.jianghu66.top

[J01] 获取当前时间
来源：http://hbd.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hen.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qch.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://ojo.hnqzz.top

TS:   new Date();  Date.now()
来源：http://epq.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xia.ehwqpu.com

Go:   time.Now()
来源：http://lme.tianlin.xyz

Ruby: Time.now
来源：http://yzx.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ofk.zdqjudy.top

[J02] 格式化输出
来源：http://inr.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aim.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bxb.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lum.yj20258888.top

TS:   d.toISOString()
来源：http://hll.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fhg.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vqc.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jum.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lvo.daxiang520.top

[J03] 字符串解析为日期
来源：http://ika.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zly.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tah.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://uli.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://cjd.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vgw.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cdw.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://gvn.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cdh.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://crf.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://awt.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uqr.ivvv.top


<!-- 参考信息 -->