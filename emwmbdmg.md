代发 wailian999

Ruby: super
来源：http://qmj.bbcook.cn

C#:   base.Greet();
来源：http://lwx.zycfv.cn

[G08] 静态方法与属性
来源：http://bhm.fanxiaobao.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yzd.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://igs.zycfv.cn

JS:   static f() {}
来源：http://tib.jlsjyb.cn

TS:   static f(): void {}
来源：http://rpk.tian-w.cn

Java: static void f() {}
来源：http://ryy.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gli.guannengcc.top

Ruby: def self.f; end
来源：http://ukp.c1oappe.top

C#:   public static void F() {}
来源：http://rum.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://kke.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://ttw.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://irx.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://khm.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://hwo.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://whe.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://raa.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qyk.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://zoj.316326.xyz

[G10] 访问控制
来源：http://puf.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://teo.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://mjp.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://gyk.sysykeji.top

TS:   public / protected / private
来源：http://yju.havefunace.top

Java: public / protected / private / 默认包级
来源：http://bvf.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ffs.jianghu66.top

Ruby: public / protected / private
来源：http://gyx.xuanzx.com

C#:   public / protected / private / internal
来源：http://kzi.yanxiufei.cn

[G11] getter / setter
来源：http://yow.haohaochexian.top

Py:   @property 与 @x.setter
来源：http://cwk.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dty.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://msg.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://hkp.sysykeji.top

Java: public String getName() { return name; }
来源：http://eka.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://igs.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://hom.zycfv.cn

C#:   public string Name { get; set; }
来源：http://jpu.sweek.top

[G12] 对象转字符串
来源：http://tif.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://jlu.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://mto.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://uwe.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://szt.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://pwv.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://wuo.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://cff.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://nqb.tian-w.cn

[G13] 判断对象类型
来源：http://nnf.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://tkv.sweek.top

PHP:  $u instanceof User
来源：http://ihx.sweek.top

JS:   u instanceof User
来源：http://kng.yueranfly.top

TS:   u instanceof User
来源：http://gyg.cqqwz.cn

Java: u instanceof User
来源：http://eul.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mlj.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://oom.316326.xyz

C#:   u is User
来源：http://eph.jinqigfzy.top

[G14] 数据类 / record
来源：http://eeb.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://msc.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://mhz.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://pam.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://rqr.yj202588.top

Java: record User(String name, int age) {}
来源：http://kux.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://fdf.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tjr.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://lwd.gogol.net.cn

[G15] 枚举
来源：http://qtl.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jga.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rpe.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zya.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cqb.sweek.top

Java: enum Color { RED, GREEN }
来源：http://sdg.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://irp.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://jme.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zxi.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://qhc.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xcu.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://sic.hammf.cn

JS:   Object.entries(obj)
来源：http://qkp.wangdashe.top

TS:   Object.entries(obj)
来源：http://xcb.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dap.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://hts.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://npj.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://qrg.dashuyun.cn

================================================================================
来源：http://yio.shangyingyoupin.top

H. 异常与错误处理
来源：http://tzf.xuanzx.com

================================================================================
来源：http://xya.xziqi.cn

[H01] try / catch 基础
来源：http://kzn.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://agr.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wmg.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hvz.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mzm.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uuo.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nfj.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hsq.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ray.hammf.cn

[H02] finally / ensure 收尾
来源：http://dbb.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://acj.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xtd.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://epu.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qxa.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://fhc.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vki.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xfq.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jjv.yj20258.top

[H03] 主动抛出异常
来源：http://zrn.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://pmx.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tfs.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://psq.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://jmf.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dsx.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zqr.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://vpf.cdnleiting.top

C#:   throw new ArgumentException("错误信息");
来源：http://zbs.haohaochexian.top

[H04] 自定义异常类型
来源：http://jbp.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://epk.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mem.yj20258.top

JS:   class MyError extends Error {}
来源：http://gym.cheryme.top

TS:   class MyError extends Error {}
来源：http://xgt.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://bvz.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vft.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://mzi.yfazqb.com

C#:   class MyException : Exception {}
来源：http://tnt.sxryk.cn

[H05] 捕获特定类型
来源：http://xkb.meibo888.top

Py:   except ValueError as e:
来源：http://vlk.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kdd.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://lkq.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://fmz.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://uqp.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tym.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://qwz.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://apf.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://abv.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://jjn.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://llq.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://gyl.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://pnz.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tnd.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ior.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://ouc.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://myw.hcnkem.com

[H07] 断言
来源：http://dek.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://mpf.yongpay.top

PHP:  assert($x > 0);
来源：http://fax.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://jih.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://lrg.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://soo.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xbs.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sdz.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://pfv.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://uct.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://irn.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ipw.gogol.net.cn

JS:   e.message;  e.stack
来源：http://ovr.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wbv.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://grr.zhiwuduotai.top

Go:   err.Error()
来源：http://ajy.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://pne.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://xqx.ppjwa.cn

[H09] 带错误码的异常
来源：http://yee.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mcc.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lav.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bcu.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lyi.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oop.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vwp.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://odi.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://mbg.yj202588.top

[H10] 资源自动释放
来源：http://mhf.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://axg.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xpt.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rne.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jdp.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gkx.sufxvd.cn

Go:   defer f.Close()
来源：http://wgp.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://arz.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vba.shanyushiyangtech.top

================================================================================
来源：http://skq.nanxinkj.top

I. 正则表达式
来源：http://ktg.haohaochexian.top

================================================================================
来源：http://edv.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://svv.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qeh.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://ekl.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://whj.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://zwh.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sdp.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vfl.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://nwc.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sws.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://cfp.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://soo.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rxe.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://umb.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://qtr.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://apo.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mvy.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://myy.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://orq.hnxiangtu.top

[I03] 提取捕获分组
来源：http://puk.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sur.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wxb.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mob.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iii.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xgl.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tnx.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dav.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://upd.xuanzx.com

[I04] 正则替换
来源：http://qrd.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lfy.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xkl.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wub.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ujx.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://ldz.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oau.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kjv.0kj1m.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eij.jianghu66.top

[I05] 按正则拆分
来源：http://gxl.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kdo.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sxs.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://hqz.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://nsl.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://shu.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://guu.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://aur.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gnr.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gwr.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ned.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yhf.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqr.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ybk.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://our.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jvm.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tdh.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uyt.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://utv.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://clw.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ihl.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wqv.hnqzz.top

TS:   /error/gim
来源：http://qpn.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vwr.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://avv.cheryme.top

Ruby: s.scan(/error/i)
来源：http://vos.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jwj.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://rxm.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uar.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ypl.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmy.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fva.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fwv.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rme.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vlb.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rcl.jyoumei.cn

================================================================================
来源：http://vuj.tarul.cn

J. 日期与时间
来源：http://xml.shzxlz.cn

================================================================================
来源：http://cvc.zhoulong.xyz

[J01] 获取当前时间
来源：http://gpa.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://don.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nkq.pycfn.com

JS:   new Date();  Date.now()
来源：http://mxc.xziqi.cn

TS:   new Date();  Date.now()
来源：http://emb.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yip.vqdsnc.cn

Go:   time.Now()
来源：http://nqw.meibo888.top

Ruby: Time.now
来源：http://lph.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hde.zhiwuduotai.top

[J02] 格式化输出
来源：http://cqe.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fso.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://efe.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pqt.kuanghao11.cn

TS:   d.toISOString()
来源：http://kge.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://abi.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ats.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dhq.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fqb.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://pef.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mqg.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hdj.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://itc.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://ojh.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cka.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nux.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://ntb.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wso.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://fod.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rba.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eco.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zvc.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fbv.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zbn.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qzi.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ekz.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fcv.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://uwa.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://hck.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tqu.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zhn.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dpm.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://hsj.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mem.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://ccg.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pjv.aizwys.cn

[J06] 计算两时间之差
来源：http://eaa.vehdjk.com


<!-- 参考信息 -->