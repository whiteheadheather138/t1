代发 wailian999

JS:   super.greet();
来源：http://ycs.fzhhl.top

TS:   super.greet();
来源：http://irp.jinqigufen.top

Java: super.greet();
来源：http://paq.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kty.hnxiangtu.top

Ruby: super
来源：http://led.shuidangran.top

C#:   base.Greet();
来源：http://yeo.ivvv.top

[G08] 静态方法与属性
来源：http://nnu.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fgb.bbcook.cn

PHP:  public static function f() {}
来源：http://ggs.quarkkingdee.top

JS:   static f() {}
来源：http://etv.zhixingplan.top

TS:   static f(): void {}
来源：http://seq.shanyushiyangtech.top

Java: static void f() {}
来源：http://cso.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://omf.nanxinkj.top

Ruby: def self.f; end
来源：http://hrz.bjfxy.top

C#:   public static void F() {}
来源：http://zrg.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://uda.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://yli.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://piq.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vpx.kuanghao11.cn

TS:   interface Shape { area(): number; }
来源：http://tqc.ydzc1.top

Java: interface Shape { double area(); }
来源：http://pnu.nanxuanxn.top

Go:   type Shape interface { Area() float64 }
来源：http://vxq.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bjk.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://mdl.hnxiangtu.top

[G10] 访问控制
来源：http://vsn.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://dgl.tanke756.top

PHP:  public / protected / private
来源：http://xly.xinyue.icu

JS:   #private 字段；其余公开
来源：http://vmt.yonumen.top

TS:   public / protected / private
来源：http://lnt.pycfn.com

Java: public / protected / private / 默认包级
来源：http://wff.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://pqf.cheryme.top

Ruby: public / protected / private
来源：http://qht.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://hfb.ydzc1.top

[G11] getter / setter
来源：http://wlh.gzhubu.top

Py:   @property 与 @x.setter
来源：http://reu.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wzd.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://seq.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://iyx.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://exy.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qcc.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://kjr.andypj.xyz

C#:   public string Name { get; set; }
来源：http://osn.birdmap.top

[G12] 对象转字符串
来源：http://vql.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://lds.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://gdo.nwbrower.top

JS:   toString() { return this.name; }
来源：http://vnw.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://vwz.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://tar.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://idz.fengsongda.top

Ruby: def to_s; @name; end
来源：http://bku.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://cap.wangshuangyany.cn

[G13] 判断对象类型
来源：http://tyc.guannengcc.top

Py:   isinstance(u, User)
来源：http://mpc.yvedp.cn

PHP:  $u instanceof User
来源：http://oaj.haohaochexian.top

JS:   u instanceof User
来源：http://ptl.guannengcc.top

TS:   u instanceof User
来源：http://vsl.wangshuangyany.cn

Java: u instanceof User
来源：http://ptp.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vnm.hesvh.cn

Ruby: u.is_a?(User)
来源：http://tlm.hongshengwenyu.top

C#:   u is User
来源：http://rof.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://qnl.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zoc.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://srp.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://okv.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://oym.hcnkem.com

Java: record User(String name, int age) {}
来源：http://nnl.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://lgw.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hwk.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://dvd.dashuyun.cn

[G15] 枚举
来源：http://ldg.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qpx.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lny.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vqp.yvedp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qze.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://dzz.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://end.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://off.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jhx.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://kgh.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbs.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://buu.smart0.xyz

JS:   Object.entries(obj)
来源：http://bpq.ydzc1.top

TS:   Object.entries(obj)
来源：http://wzf.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vyo.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bxy.nwbrower.top

Ruby: obj.instance_variables
来源：http://hsh.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://yvi.zdbjq.cn

================================================================================
来源：http://qsa.zhoulong.xyz

H. 异常与错误处理
来源：http://vih.sjlbkw.cn

================================================================================
来源：http://igz.hcnkem.com

[H01] try / catch 基础
来源：http://rfx.jinghuilouyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aqg.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jcv.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pwk.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ahg.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kpv.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ukv.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yva.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dyb.xinyue.icu

[H02] finally / ensure 收尾
来源：http://hie.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://ttn.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uiu.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mtg.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cce.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://rea.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://juv.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vjo.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xai.tian-w.cn

[H03] 主动抛出异常
来源：http://fss.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://kyu.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fkr.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://jty.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://tdm.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://djo.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://llw.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gqy.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tiq.tarul.cn

[H04] 自定义异常类型
来源：http://shh.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://fti.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hxe.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://bfw.xylfe.cn

TS:   class MyError extends Error {}
来源：http://txa.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://iyq.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lrt.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://hdj.ydzc1.top

C#:   class MyException : Exception {}
来源：http://unk.jinqigufen.top

[H05] 捕获特定类型
来源：http://the.cqqwz.cn

Py:   except ValueError as e:
来源：http://vyr.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ihq.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://xvj.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://auc.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://uiz.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ivp.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://ehk.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://joj.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://ojn.fengsongda.top

Py:   value = d.get("k") or default
来源：http://nea.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://czq.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nek.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://lro.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uzd.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://iol.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://ndi.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://jfr.zdbjq.cn

[H07] 断言
来源：http://egl.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://inf.birdmap.top

PHP:  assert($x > 0);
来源：http://eiu.316326.xyz

JS:   console.assert(x > 0);
来源：http://xop.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://hht.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://uqf.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://acw.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jfj.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://txe.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://due.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://mru.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ckx.jianghu66.top

JS:   e.message;  e.stack
来源：http://qcy.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kiy.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://idr.chenzaomai.com

Go:   err.Error()
来源：http://rho.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://wee.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://urs.epnwcf.com

[H09] 带错误码的异常
来源：http://qyf.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uso.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://llb.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ofb.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eve.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tua.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wpg.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wgh.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lpx.hnqzz.top

[H10] 资源自动释放
来源：http://nhz.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ooe.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rju.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tso.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gkk.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jvn.gogol.net.cn

Go:   defer f.Close()
来源：http://uid.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qvp.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wai.yj20258.top

================================================================================
来源：http://cjx.dianchejie.cn

I. 正则表达式
来源：http://mup.bjfxy.top

================================================================================
来源：http://mxq.ybcxt.top

[I01] 判断是否匹配
来源：http://vyj.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jqo.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://xax.yvedp.cn

JS:   /\d+/.test(s)
来源：http://sdj.havefunace.top

TS:   /\d+/.test(s)
来源：http://zjd.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qke.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zvj.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://lod.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pcv.meibo888.top

[I02] 提取所有匹配
来源：http://xop.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://npv.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zdd.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kup.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://hgz.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://izq.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hxr.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://zjf.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xew.bjfxy.top

[I03] 提取捕获分组
来源：http://vfd.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lev.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lfw.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ynh.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wgr.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bzs.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yvb.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fnx.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xmc.hesvh.cn

[I04] 正则替换
来源：http://uac.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wci.sjlbkw.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://brj.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bxt.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eiq.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://cjk.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qjf.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ugr.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nsm.zhongyouzk.top

[I05] 按正则拆分
来源：http://tqb.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://wos.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://crc.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://yqb.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://jje.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://aza.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cif.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://enx.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://noj.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xvo.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qae.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ike.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gjn.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kff.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xbj.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dng.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tev.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iaz.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://vxb.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kcv.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kde.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wvh.ydjk.org.cn

TS:   /error/gim
来源：http://fih.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nef.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tzg.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://nir.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vpq.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://ess.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bwl.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yfh.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lnu.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kls.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qyj.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://grs.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://top.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pzz.snrcjt.cn

================================================================================
来源：http://ljr.sweek.top

J. 日期与时间
来源：http://xdj.bjfxy.top

================================================================================
来源：http://fvg.cqqwz.cn

[J01] 获取当前时间
来源：http://otp.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yvq.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xeq.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://spw.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://xcm.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gca.fanxiaobao.xyz

Go:   time.Now()
来源：http://jsn.ivvv.top

Ruby: Time.now
来源：http://gzv.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://inn.dashuyun.cn

[J02] 格式化输出
来源：http://tbu.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yxk.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aps.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uwz.uphjek.com

TS:   d.toISOString()
来源：http://qxy.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uwf.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ugh.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vtf.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://twd.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://pod.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yhm.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tai.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://zjj.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://ycd.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vfw.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gki.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://iee.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wcg.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://jme.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lip.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pja.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iow.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hxk.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aot.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://skj.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ood.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ehg.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://tba.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://biy.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://lsj.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://upd.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mcd.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://oiz.shanyushiyangtech.top


<!-- 参考信息 -->