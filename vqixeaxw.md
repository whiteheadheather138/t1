代发 wailian999

PHP:  public static function f() {}
来源：http://jur.zhoulong.xyz

JS:   static f() {}
来源：http://nxs.hammf.cn

TS:   static f(): void {}
来源：http://zcb.jinghuilouyu.cn

Java: static void f() {}
来源：http://wes.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://vyn.iojbl.cn

Ruby: def self.f; end
来源：http://wth.yongpay.top

C#:   public static void F() {}
来源：http://oib.cheryme.top

[G09] 接口 / 抽象类
来源：http://zly.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://jlu.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lor.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qvu.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://lie.guannengcc.top

Java: interface Shape { double area(); }
来源：http://skm.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://jdp.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gzh.sweek.top

C#:   interface IShape { double Area(); }
来源：http://zmp.yanxiufei.cn

[G10] 访问控制
来源：http://pqa.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://qrw.hysaishi.cn

PHP:  public / protected / private
来源：http://cve.cashguo.top

JS:   #private 字段；其余公开
来源：http://cak.shzxlz.cn

TS:   public / protected / private
来源：http://ohe.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://iww.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kcc.hesvh.cn

Ruby: public / protected / private
来源：http://fhr.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://wbc.ivvv.top

[G11] getter / setter
来源：http://jxb.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://jte.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cll.c1oappe.top

JS:   get name() { return this._name; }
来源：http://ego.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://hap.hammf.cn

Java: public String getName() { return name; }
来源：http://zor.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://paw.iojbl.cn

Ruby: attr_accessor :name
来源：http://uza.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://qfe.svipenyu.cn

[G12] 对象转字符串
来源：http://pho.yj20258.top

Py:   def __str__(self): return self.name
来源：http://ssq.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://soz.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://fos.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://bkx.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://ksx.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://mid.52xcode.cn

Ruby: def to_s; @name; end
来源：http://uqu.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://dtl.tarul.cn

[G13] 判断对象类型
来源：http://grg.chenlongwang.top

Py:   isinstance(u, User)
来源：http://tef.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://qid.sysykeji.top

JS:   u instanceof User
来源：http://jvb.iojbl.cn

TS:   u instanceof User
来源：http://chi.svipenyu.cn

Java: u instanceof User
来源：http://jgw.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://dwh.cheryme.top

Ruby: u.is_a?(User)
来源：http://pjf.zycfv.cn

C#:   u is User
来源：http://onv.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://ggw.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nbu.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://dem.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://ixo.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://wrd.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://hzc.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://mpk.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pur.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://cxa.tianlin.xyz

[G15] 枚举
来源：http://tyf.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ybu.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://als.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://izp.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://suk.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://ofp.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hcj.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://iwf.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vhx.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://xyt.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wcs.andypj.xyz

PHP:  get_object_vars($obj);
来源：http://ove.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://guw.jyoumei.cn

TS:   Object.entries(obj)
来源：http://gdj.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gcu.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jnd.sysykeji.top

Ruby: obj.instance_variables
来源：http://wih.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://blp.gzhubu.top

================================================================================
来源：http://sqy.yanxiufei.cn

H. 异常与错误处理
来源：http://crk.aizwys.cn

================================================================================
来源：http://kcs.zdbjq.cn

[H01] try / catch 基础
来源：http://sdr.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kcz.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ucd.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zrc.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lut.gaohongyu789.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fex.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tar.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zmn.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sov.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://sqe.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ezw.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://gxk.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vfc.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sou.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://ngw.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jsq.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yrj.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ewm.birdmap.top

[H03] 主动抛出异常
来源：http://bzw.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://rwj.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fst.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://ayx.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://msa.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mpz.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zob.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hzd.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://pmb.guowangkeji.top

[H04] 自定义异常类型
来源：http://aeo.yj202588.top

Py:   class MyError(Exception): pass
来源：http://jem.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lsr.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://tut.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://wmd.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://rfc.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kbp.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://ecz.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://iwj.meibo888.top

[H05] 捕获特定类型
来源：http://odf.zhoulong.xyz

Py:   except ValueError as e:
来源：http://kgk.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jde.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://ggb.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://zdj.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://uhy.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nbn.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://jxu.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cav.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://neu.smart0.xyz

Py:   value = d.get("k") or default
来源：http://qfw.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ugw.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://juz.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://qen.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wnp.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wrg.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://boh.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://euz.yj20258888.top

[H07] 断言
来源：http://fjx.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://xbk.xuanzx.com

PHP:  assert($x > 0);
来源：http://wsd.yfazqb.com

JS:   console.assert(x > 0);
来源：http://pis.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://zst.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://qvm.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nzr.yuanzhike.top

Ruby: raise "必须为正" unless x > 0
来源：http://ybu.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://apf.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://hzu.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://maw.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dcj.jiagoushi.top

JS:   e.message;  e.stack
来源：http://ewb.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vin.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://loo.yonumen.top

Go:   err.Error()
来源：http://lpd.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://nui.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://lrm.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://gcf.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hqh.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://clb.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cof.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://asw.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dkk.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zvq.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aeh.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://oop.feifeiyinyue.top

[H10] 资源自动释放
来源：http://ots.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://oie.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://utd.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mxw.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lpu.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lrt.nanxinkj.top

Go:   defer f.Close()
来源：http://hpv.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rvk.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tpk.hnxiangtu.top

================================================================================
来源：http://pcf.jiagoushi.top

I. 正则表达式
来源：http://zij.chenlongwang.top

================================================================================
来源：http://iyq.shzxlz.cn

[I01] 判断是否匹配
来源：http://fir.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ien.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hpx.zycfv.cn

JS:   /\d+/.test(s)
来源：http://crs.yj202588.top

TS:   /\d+/.test(s)
来源：http://woa.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eng.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pza.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://zrl.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pjb.daxiang520.top

[I02] 提取所有匹配
来源：http://vkm.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://atw.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://syz.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dfx.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://bwt.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cwc.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xde.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://alp.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://idm.quarkkingdee.top

[I03] 提取捕获分组
来源：http://elj.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hfj.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://msd.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vyh.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tsv.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uem.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bod.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wto.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://svm.jinghuilouyu.cn

[I04] 正则替换
来源：http://pbs.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qgu.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cte.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://vka.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://evc.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rgm.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aqr.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jfh.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pcd.jianghu66.top

[I05] 按正则拆分
来源：http://kwj.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qrj.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xxf.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://zlp.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://haj.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://heb.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tlt.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ogp.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iqb.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cqc.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://liz.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://djd.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zvn.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rno.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qbj.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rcu.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nnc.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dei.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://fdb.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://psw.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mak.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wrz.hfpthk.cn

TS:   /error/gim
来源：http://bbf.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lhu.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iol.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://pza.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jpx.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://qwh.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wla.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fly.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lcy.ehwqpu.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aei.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://grp.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kjw.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pas.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dvi.zhijiandao.cn

================================================================================
来源：http://zhy.zhaomingkeji.xyz

J. 日期与时间
来源：http://sds.yj202588.top

================================================================================
来源：http://rco.daxiang520.top

[J01] 获取当前时间
来源：http://qch.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qcy.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lls.fehbvm.com

JS:   new Date();  Date.now()
来源：http://kgb.yueranfly.top

TS:   new Date();  Date.now()
来源：http://bga.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jyr.yanxiufei.cn

Go:   time.Now()
来源：http://msq.hcnkem.com

Ruby: Time.now
来源：http://bro.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hme.birdmap.top

[J02] 格式化输出
来源：http://eig.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oqg.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rym.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://htb.shzxlz.cn

TS:   d.toISOString()
来源：http://suy.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://plw.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bdn.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mkf.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pro.ydzc1.top

[J03] 字符串解析为日期
来源：http://isf.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdw.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://olx.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://vpj.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://vnw.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://lym.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tss.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://fue.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wjo.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://bix.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eem.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://esb.gaohongyu789.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bpx.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://esc.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pku.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gkp.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nau.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ufs.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://ltv.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://jcq.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yoj.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lhx.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eua.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://xsu.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ykg.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://bnp.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://idq.vqdsnc.cn

[J06] 计算两时间之差
来源：http://hkk.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://rid.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://uas.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://shr.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nxb.meibo888.top


<!-- 参考信息 -->