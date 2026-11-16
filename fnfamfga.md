代发 wailian999

JS:   super.greet();
来源：http://ujd.ydjk.org.cn

TS:   super.greet();
来源：http://dhw.aizwys.cn

Java: super.greet();
来源：http://wci.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ryo.ydzc1.top

Ruby: super
来源：http://qol.gotoacloud.top

C#:   base.Greet();
来源：http://xju.jinqigufen.top

[G08] 静态方法与属性
来源：http://ksm.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oov.birdmap.top

PHP:  public static function f() {}
来源：http://yuc.jianghu66.top

JS:   static f() {}
来源：http://sjf.fengsongda.top

TS:   static f(): void {}
来源：http://fww.tarul.cn

Java: static void f() {}
来源：http://nhs.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cxe.hammf.cn

Ruby: def self.f; end
来源：http://ydz.bbcook.cn

C#:   public static void F() {}
来源：http://dmc.sweek.top

[G09] 接口 / 抽象类
来源：http://iaw.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://qtl.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://fdv.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tct.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://nmz.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://fjc.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://uhv.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://chd.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://igj.andypj.xyz

[G10] 访问控制
来源：http://cfe.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://zbh.chenjidiqi.icu

PHP:  public / protected / private
来源：http://psb.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://nbs.jiagoushi.top

TS:   public / protected / private
来源：http://iye.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://vpw.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yfb.yvedp.cn

Ruby: public / protected / private
来源：http://aju.sxryk.cn

C#:   public / protected / private / internal
来源：http://wak.meibo888.top

[G11] getter / setter
来源：http://pqv.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://unu.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://qka.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://nwy.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://lhq.yuanzhike.top

Java: public String getName() { return name; }
来源：http://aux.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mzi.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://sbz.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://hlf.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://pnr.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://ecb.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://daw.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://dph.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://nwd.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://kmo.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://osg.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://ipm.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://xon.9152youxi.cn

[G13] 判断对象类型
来源：http://fvu.jqgfzy.top

Py:   isinstance(u, User)
来源：http://mpc.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://fql.shzxlz.cn

JS:   u instanceof User
来源：http://msc.jinghuilouyu.cn

TS:   u instanceof User
来源：http://qak.fzhhl.top

Java: u instanceof User
来源：http://kgr.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tpr.hesvh.cn

Ruby: u.is_a?(User)
来源：http://dnv.wangdashe.top

C#:   u is User
来源：http://olk.hywenlv.cn

[G14] 数据类 / record
来源：http://hmo.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dac.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://jzi.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://ahy.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://map.birdmap.top

Java: record User(String name, int age) {}
来源：http://ksc.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://fqa.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lxk.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://pam.redwolf501.top

[G15] 枚举
来源：http://gfd.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://twt.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://muu.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://svj.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tmg.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://ive.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yru.ydjk.org.cn

Ruby: Color = %i[red green].freeze
来源：http://zmx.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mev.uphjek.com

[G16] 对象转数组 / 字典
来源：http://veh.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zrx.yonumen.top

PHP:  get_object_vars($obj);
来源：http://kkf.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://nnh.iojbl.cn

TS:   Object.entries(obj)
来源：http://blt.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://egc.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fvg.nanxinkj.top

Ruby: obj.instance_variables
来源：http://kol.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://uqu.jinqigufen.top

================================================================================
来源：http://gwn.aibaodan.cn

H. 异常与错误处理
来源：http://mtu.dashuyun.cn

================================================================================
来源：http://ygr.zhongyouzk.top

[H01] try / catch 基础
来源：http://dvy.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bdc.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uti.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eve.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ckl.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ded.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ocj.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ncl.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://how.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://ufu.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://ljj.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mnr.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mol.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mva.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tda.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fge.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gpn.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nrg.jinqigufen.top

[H03] 主动抛出异常
来源：http://tkt.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://vft.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ubu.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://zvl.tarul.cn

TS:   throw new Error("错误信息");
来源：http://swb.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://iml.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qsi.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uvt.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ypr.xziqi.cn

[H04] 自定义异常类型
来源：http://gps.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://rlm.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://uhk.wangdashe.top

JS:   class MyError extends Error {}
来源：http://pyo.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://cxk.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://zzl.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hgw.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://jxo.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://jsu.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://kgp.ydjk.org.cn

Py:   except ValueError as e:
来源：http://vvv.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rwg.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://hun.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://fkt.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://ajc.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fjn.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://ehk.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://len.yongpay.top

[H06] 可选值 / 空值安全访问
来源：http://qut.cucudq.cn

Py:   value = d.get("k") or default
来源：http://ptf.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://jts.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xtu.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://pjo.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sjk.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hjk.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://nix.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://rlt.hywenlv.cn

[H07] 断言
来源：http://xnj.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://djq.yangfankeji.com

PHP:  assert($x > 0);
来源：http://yaw.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://zsx.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://hjz.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://prg.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zbs.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://kuf.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://gfw.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://tgm.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://vmv.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lny.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://zoy.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ssq.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ved.52xcode.cn

Go:   err.Error()
来源：http://eid.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://atm.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://mgt.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://xep.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://frv.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qiw.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szx.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rmk.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ssy.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://abo.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ter.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nwb.sysykeji.top

[H10] 资源自动释放
来源：http://nlo.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vyr.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zxu.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xbo.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gca.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oqa.zhiwuduotai.top

Go:   defer f.Close()
来源：http://wzq.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pgf.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zkc.hnxiangtu.top

================================================================================
来源：http://pwv.meibo888.top

I. 正则表达式
来源：http://scu.shangyingyoupin.top

================================================================================
来源：http://lev.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://irg.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kxr.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vrh.sweek.top

JS:   /\d+/.test(s)
来源：http://tse.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://lxy.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ngt.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wpi.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://phb.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lol.0kj1m.cn

[I02] 提取所有匹配
来源：http://mla.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://syr.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ppz.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://exe.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://bgz.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kjd.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://umf.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://ioi.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gid.zhongyouzk.top

[I03] 提取捕获分组
来源：http://vvy.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vjg.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gaa.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xoc.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xyg.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://opg.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uzj.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://koq.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zzm.chenjidiqi.icu

[I04] 正则替换
来源：http://ixn.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jge.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sho.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://tal.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://gvj.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qhq.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wmo.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jbp.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eeh.hnqzz.top

[I05] 按正则拆分
来源：http://vyv.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bre.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eeb.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://okm.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://fep.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://hlo.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tcg.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://djv.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://acl.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fpl.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gxi.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://foq.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yjb.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://anr.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nnb.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ouj.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wsm.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ekh.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://ybc.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qia.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rhf.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://afv.c1oappe.top

TS:   /error/gim
来源：http://qpe.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nlc.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lpe.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://uop.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://brp.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://zaq.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ctx.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wkv.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://txg.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://inw.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oli.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jwr.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zvb.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cpk.xylfe.cn

================================================================================
来源：http://lqc.xinyue.icu

J. 日期与时间
来源：http://cfp.wangdashe.top

================================================================================
来源：http://doj.hnxiangtu.top

[J01] 获取当前时间
来源：http://xec.hywenlv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xnn.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lvu.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://wje.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://vtx.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://lym.vqdsnc.cn

Go:   time.Now()
来源：http://rus.shangyingyoupin.top

Ruby: Time.now
来源：http://css.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iwa.guowangkeji.top

[J02] 格式化输出
来源：http://guz.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ghb.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://myj.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lvd.jqgfzy.top

TS:   d.toISOString()
来源：http://hyb.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vkl.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://prg.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lmp.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qbz.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://rfr.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://haw.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qfg.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://sey.sweek.top

TS:   new Date("2024-01-02")
来源：http://idt.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://ehy.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tng.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://fil.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kpz.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://rmb.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baz.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iow.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rdk.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ksc.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ias.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zle.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ltr.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fwu.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://lcj.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://gkl.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://scm.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rgx.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jqa.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://hvq.hnxiangtu.top


<!-- 参考信息 -->