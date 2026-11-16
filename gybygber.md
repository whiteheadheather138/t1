代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://ytz.fzhhl.top

[G07] 调用父类方法
来源：http://cvk.aizwys.cn

Py:   super().greet()
来源：http://lqv.ctjpmb.com

PHP:  parent::greet();
来源：http://wgh.hywenlv.cn

JS:   super.greet();
来源：http://pkr.snrcjt.cn

TS:   super.greet();
来源：http://oud.sjlbkw.cn

Java: super.greet();
来源：http://fgo.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hyy.chenjidiqi.icu

Ruby: super
来源：http://jwj.guannengcc.top

C#:   base.Greet();
来源：http://sba.hammf.cn

[G08] 静态方法与属性
来源：http://dsn.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://siz.tarul.cn

PHP:  public static function f() {}
来源：http://xdw.jyoumei.cn

JS:   static f() {}
来源：http://rqn.vehdjk.com

TS:   static f(): void {}
来源：http://muu.vehdjk.com

Java: static void f() {}
来源：http://wra.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mnh.shzxlz.cn

Ruby: def self.f; end
来源：http://ogx.yj20258.top

C#:   public static void F() {}
来源：http://voi.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://vxk.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://kcc.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://glj.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dmr.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://yoe.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://qkc.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://tpa.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pco.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://ond.0kj1m.cn

[G10] 访问控制
来源：http://twh.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://pls.yongpay.top

PHP:  public / protected / private
来源：http://pgx.fzhhl.top

JS:   #private 字段；其余公开
来源：http://tml.xinyue.icu

TS:   public / protected / private
来源：http://xjs.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://pud.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zyg.316326.xyz

Ruby: public / protected / private
来源：http://rkj.xylfe.cn

C#:   public / protected / private / internal
来源：http://hol.xylfe.cn

[G11] getter / setter
来源：http://nke.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://lgm.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://igv.zhaomingkeji.xyz

JS:   get name() { return this._name; }
来源：http://axn.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://ebv.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://xvu.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cup.tianlin.xyz

Ruby: attr_accessor :name
来源：http://hyb.xuanzx.com

C#:   public string Name { get; set; }
来源：http://uep.vehdjk.com

[G12] 对象转字符串
来源：http://kgw.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://ega.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rhd.cucudq.cn

JS:   toString() { return this.name; }
来源：http://qzy.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://ysm.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://law.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ocs.316326.xyz

Ruby: def to_s; @name; end
来源：http://xeb.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://kap.cdnleiting.top

[G13] 判断对象类型
来源：http://akl.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://doz.yonumen.top

PHP:  $u instanceof User
来源：http://ahn.chenlongwang.top

JS:   u instanceof User
来源：http://cxt.daxiang520.top

TS:   u instanceof User
来源：http://aev.yj202588.top

Java: u instanceof User
来源：http://dsu.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ruo.yj202588.top

Ruby: u.is_a?(User)
来源：http://vbz.epnwcf.com

C#:   u is User
来源：http://dnt.fanxiaobao.xyz

[G14] 数据类 / record
来源：http://kwy.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ctw.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://pdl.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://jdw.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://wqd.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://lwl.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://mkd.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nii.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://qxq.jinqigfzy.top

[G15] 枚举
来源：http://xcg.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ire.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ijb.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kdd.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vsw.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://kil.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ddz.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://pmc.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mdb.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://zmh.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yrj.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://hxe.sysykeji.top

JS:   Object.entries(obj)
来源：http://itg.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://wwn.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sqr.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://boa.yj20258.top

Ruby: obj.instance_variables
来源：http://pcp.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://kut.zycfv.cn

================================================================================
来源：http://vkx.pengpengdd.cyou

H. 异常与错误处理
来源：http://gpp.hfpthk.cn

================================================================================
来源：http://lsc.hesvh.cn

[H01] try / catch 基础
来源：http://njj.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qwf.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ocj.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://joo.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cvu.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bxe.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uns.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hye.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bnp.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://tzn.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://igk.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tqp.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dgn.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rtd.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yhi.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://zfu.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://gwl.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bkb.cashguo.top

[H03] 主动抛出异常
来源：http://zld.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://wsy.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fnb.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://mox.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://tre.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mhh.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ayv.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://gqi.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://nof.nanxuanxn.top

[H04] 自定义异常类型
来源：http://lpr.birdmap.top

Py:   class MyError(Exception): pass
来源：http://piz.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nfe.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://jdt.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://yab.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://ykv.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kyw.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://dhd.gzhubu.top

C#:   class MyException : Exception {}
来源：http://qiy.yangfankeji.com

[H05] 捕获特定类型
来源：http://qmt.cqqwz.cn

Py:   except ValueError as e:
来源：http://ayp.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://elo.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://sjs.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://lyh.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://aiz.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uhq.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://ylt.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://psd.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://wjm.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://dyw.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://fod.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://kkd.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://ckq.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wzh.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://duu.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://ang.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://xov.yuxming.cn

[H07] 断言
来源：http://jjn.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://tjh.hesvh.cn

PHP:  assert($x > 0);
来源：http://lvo.jinyuanbaomall.cn

JS:   console.assert(x > 0);
来源：http://efm.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://aht.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://wro.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cjs.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://rzb.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://dsd.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://tgl.zdqjudy.top

Py:   str(e);  traceback.format_exc()
来源：http://vor.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rym.cqqwz.cn

JS:   e.message;  e.stack
来源：http://kpi.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cht.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wzg.shangyingyoupin.top

Go:   err.Error()
来源：http://nxv.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://nef.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://zxq.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://ztx.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gzw.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vou.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dpa.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lzl.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sje.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hqp.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://xob.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gxj.52xcode.cn

[H10] 资源自动释放
来源：http://sdq.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ihw.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xob.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nma.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zyn.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xwg.fehbvm.com

Go:   defer f.Close()
来源：http://xfh.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gnq.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mab.c1oappe.top

================================================================================
来源：http://tvc.jinqigufen.top

I. 正则表达式
来源：http://bic.nanxinkj.top

================================================================================
来源：http://opy.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://qgt.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hiy.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yyt.xinyue.icu

JS:   /\d+/.test(s)
来源：http://hpy.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://jbj.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://quy.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ijg.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://ckj.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cio.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://pih.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://yho.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oqj.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hld.yongpay.top

TS:   s.match(/\d+/g)
来源：http://piw.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wtu.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iev.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://vgh.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jyr.xziqi.cn

[I03] 提取捕获分组
来源：http://meg.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://voi.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xbb.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://exd.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mxq.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gku.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nap.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wlg.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://css.yvedp.cn

[I04] 正则替换
来源：http://hvt.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://svd.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rgw.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://ipk.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gll.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://fhb.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gmx.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lsl.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gdn.gogol.net.cn

[I05] 按正则拆分
来源：http://wdk.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dvr.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ddp.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://ecl.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://wfn.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://wwm.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fwb.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://zlr.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ymo.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dfv.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qfv.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rre.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://erx.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aox.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kra.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jel.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cyt.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wre.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://keg.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yot.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kff.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mve.ydjk.org.cn

TS:   /error/gim
来源：http://nza.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://civ.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yct.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://yqy.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ztb.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://xco.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ssj.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ioz.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://esc.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xlx.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ofo.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bvr.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kcz.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gmc.nanxinkj.top

================================================================================
来源：http://spt.yuxming.cn

J. 日期与时间
来源：http://gcr.jqgfzy.top

================================================================================
来源：http://qjd.pycfn.com

[J01] 获取当前时间
来源：http://ott.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://rbu.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ehl.sweek.top

JS:   new Date();  Date.now()
来源：http://yeg.epnwcf.com

TS:   new Date();  Date.now()
来源：http://xee.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ohu.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://auf.zhoulong.xyz

Ruby: Time.now
来源：http://eso.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rji.zhijiandao.cn

[J02] 格式化输出
来源：http://wqi.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cdg.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jfa.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dbg.jinqigufen.top

TS:   d.toISOString()
来源：http://nad.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gan.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ubs.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzd.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ctu.epnwcf.com

[J03] 字符串解析为日期
来源：http://dwh.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ajx.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://etz.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://jvh.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://jxg.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://lyk.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nyq.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://zts.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tqa.hcnkem.com

[J04] 时间戳与日期互转
来源：http://rht.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qlp.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ali.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ntk.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fpq.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zrg.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tno.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cmy.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nhm.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://rdw.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://dut.ybcxt.top


<!-- 参考信息 -->