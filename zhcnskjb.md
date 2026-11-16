代发 wailian999

Ruby: super
来源：http://abb.yj20258.top

C#:   base.Greet();
来源：http://zod.gzhubu.top

[G08] 静态方法与属性
来源：http://gdv.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://brp.guannengcc.top

PHP:  public static function f() {}
来源：http://eex.tarul.cn

JS:   static f() {}
来源：http://pyo.jinqigufen.top

TS:   static f(): void {}
来源：http://xdk.andypj.xyz

Java: static void f() {}
来源：http://fwb.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kfy.jyoumei.cn

Ruby: def self.f; end
来源：http://myi.cheryme.top

C#:   public static void F() {}
来源：http://bhv.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://ged.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://cpk.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://ypi.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dsd.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://cxc.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://eyi.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://izo.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://adc.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://yqf.sufxvd.cn

[G10] 访问控制
来源：http://mjb.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://bod.9152youxi.cn

PHP:  public / protected / private
来源：http://qzt.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://gat.yj20258.top

TS:   public / protected / private
来源：http://xlj.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://etz.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://whf.smart0.xyz

Ruby: public / protected / private
来源：http://gya.nanxinkj.top

C#:   public / protected / private / internal
来源：http://kxg.birdmap.top

[G11] getter / setter
来源：http://jub.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://jta.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://jhp.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://ewc.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://hzf.chenzaomai.com

Java: public String getName() { return name; }
来源：http://cgd.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mkh.fengsongda.top

Ruby: attr_accessor :name
来源：http://tkh.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://wcl.fengsongda.top

[G12] 对象转字符串
来源：http://vel.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://vpy.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nek.wangdashe.top

JS:   toString() { return this.name; }
来源：http://rpj.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://nac.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://scy.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://zgx.bbcook.cn

Ruby: def to_s; @name; end
来源：http://gcq.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://pwj.cqqwz.cn

[G13] 判断对象类型
来源：http://tvs.316326.xyz

Py:   isinstance(u, User)
来源：http://uhg.hnqzz.top

PHP:  $u instanceof User
来源：http://pbf.yuxming.cn

JS:   u instanceof User
来源：http://dlo.hesvh.cn

TS:   u instanceof User
来源：http://use.shanyushiyangtech.top

Java: u instanceof User
来源：http://bbu.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zhj.jianghu66.top

Ruby: u.is_a?(User)
来源：http://pod.vehdjk.com

C#:   u is User
来源：http://emn.zhoulong.xyz

[G14] 数据类 / record
来源：http://tff.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://omi.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://ghp.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://scf.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://kaw.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://dfk.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://cdu.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yte.birdmap.top

C#:   record User(string Name, int Age);
来源：http://zub.hesvh.cn

[G15] 枚举
来源：http://rwz.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sqf.vehdjk.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://rfl.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rfz.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jqw.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://iri.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uxi.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://coz.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://adp.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://udx.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tlg.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://bse.snrcjt.cn

JS:   Object.entries(obj)
来源：http://dcj.epnwcf.com

TS:   Object.entries(obj)
来源：http://crn.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vyl.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gyd.zhixingplan.top

Ruby: obj.instance_variables
来源：http://lri.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://zvn.sysykeji.top

================================================================================
来源：http://pvo.nanxinkj.top

H. 异常与错误处理
来源：http://ifx.yongpay.top

================================================================================
来源：http://wzr.gaohongyu789.top

[H01] try / catch 基础
来源：http://mvl.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cun.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nph.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://npf.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqp.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gxi.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wuf.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://itp.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lgn.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://nsv.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qci.redwolf501.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ujy.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hzg.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://khq.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://ytz.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://iql.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hvj.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mtz.nanxuanxn.top

[H03] 主动抛出异常
来源：http://mgj.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://naz.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qoc.tarul.cn

JS:   throw new Error("错误信息");
来源：http://vnq.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://bam.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mzu.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iwb.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fke.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iuk.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://vbx.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://vfg.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wpo.yfazqb.com

JS:   class MyError extends Error {}
来源：http://nwt.fktsv.cn

TS:   class MyError extends Error {}
来源：http://obd.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://qvu.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mtv.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://hxd.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://oxt.cqqwz.cn

[H05] 捕获特定类型
来源：http://mml.havefunace.top

Py:   except ValueError as e:
来源：http://cce.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qpz.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://jqe.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://zgw.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://cuu.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bol.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://wzn.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nmp.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://jmm.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://wku.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://sab.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://olv.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wkc.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sak.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ezz.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://aob.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://zli.yj202588.top

[H07] 断言
来源：http://zna.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://trg.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://udw.yvedp.cn

JS:   console.assert(x > 0);
来源：http://hpj.redwolf501.top

TS:   console.assert(x > 0);
来源：http://fdw.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://bja.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wzn.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://zkk.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://vnf.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://twj.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://wjk.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mxv.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://qbb.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zfw.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://iyh.ppjwa.cn

Go:   err.Error()
来源：http://zsq.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://ete.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://yxx.bjfxy.top

[H09] 带错误码的异常
来源：http://uxb.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gps.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ncq.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jli.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wgc.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jzr.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uvi.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eus.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bsz.hfpthk.cn

[H10] 资源自动释放
来源：http://rvn.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hmp.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qxy.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ayk.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gml.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://opx.jinqigfzy.top

Go:   defer f.Close()
来源：http://jon.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pij.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://brj.redwolf501.top

================================================================================
来源：http://qaa.birdmap.top

I. 正则表达式
来源：http://zih.shuidangran.top

================================================================================
来源：http://sps.bjfxy.top

[I01] 判断是否匹配
来源：http://oge.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pqg.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vbo.epnwcf.com

JS:   /\d+/.test(s)
来源：http://gxq.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://ecf.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mhw.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pvo.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://sgw.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://egc.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://roy.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://hqn.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lil.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ukt.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://fsh.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://joj.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kzi.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://alp.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hao.0kj1m.cn

[I03] 提取捕获分组
来源：http://sif.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://woh.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zng.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uud.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://osy.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fvg.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xfg.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bsa.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aby.xuanzx.com

[I04] 正则替换
来源：http://kxm.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ond.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dit.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://vhs.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://qmm.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://umy.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xyt.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tff.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ajr.jinqigfzy.top

[I05] 按正则拆分
来源：http://ikt.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lrv.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dvy.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://qxp.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://bfn.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://wlx.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lii.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sbd.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gmz.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dvt.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zxm.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mbc.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jcs.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pvt.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://imm.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ray.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qfj.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jjn.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://nvo.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bfp.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bpb.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kwv.ywan-chungtsiang.top

TS:   /error/gim
来源：http://kwv.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ccd.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://asv.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://otn.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zso.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://zia.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ged.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ybw.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://teq.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pny.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ext.ybcxt.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xnb.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mfq.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vib.zhoulong.xyz

================================================================================
来源：http://vcb.nanxinkj.top

J. 日期与时间
来源：http://ram.fehbvm.com

================================================================================
来源：http://fmu.ctjpmb.com

[J01] 获取当前时间
来源：http://xhi.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://iam.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fcz.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://aqc.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://axe.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qin.andypj.xyz

Go:   time.Now()
来源：http://krm.chenlongwang.top

Ruby: Time.now
来源：http://kkw.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hfq.yongpay.top

[J02] 格式化输出
来源：http://cvx.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xvi.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://egt.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kko.feifeiyinyue.top

TS:   d.toISOString()
来源：http://vaq.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://prw.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://epf.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yoe.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lmp.yvedp.cn

[J03] 字符串解析为日期
来源：http://kqt.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fek.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yen.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://lzx.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://por.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kde.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uyh.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://yfv.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://svf.316326.xyz

[J04] 时间戳与日期互转
来源：http://mzb.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lof.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nbt.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ijw.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://itr.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pno.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pbw.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://orf.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wss.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://agy.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://els.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kvc.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgd.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pyr.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://owi.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://asw.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://oul.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xfg.zycfv.cn

[J06] 计算两时间之差
来源：http://sqb.xuetiantiany.cn


<!-- 参考信息 -->