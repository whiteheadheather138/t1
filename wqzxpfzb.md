代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://pvv.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hdc.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bwf.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://wzd.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://tms.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://ihk.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kko.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://uiq.cdnleiting.top

[G10] 访问控制
来源：http://yio.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://lat.cheryme.top

PHP:  public / protected / private
来源：http://sru.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://baz.fanxiaobao.xyz

TS:   public / protected / private
来源：http://qwj.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://cic.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zub.wangdashe.top

Ruby: public / protected / private
来源：http://fie.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://bks.hysaishi.cn

[G11] getter / setter
来源：http://qve.sxryk.cn

Py:   @property 与 @x.setter
来源：http://enw.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mei.bbcook.cn

JS:   get name() { return this._name; }
来源：http://nio.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://sjx.snrcjt.cn

Java: public String getName() { return name; }
来源：http://epx.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ywf.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://jao.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://gya.zdqjudy.top

[G12] 对象转字符串
来源：http://qdj.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://dcx.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lia.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://rvu.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://tze.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://dnk.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wzm.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://uss.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://aut.0kj1m.cn

[G13] 判断对象类型
来源：http://syt.yfazqb.com

Py:   isinstance(u, User)
来源：http://hui.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://fzn.dianchejie.cn

JS:   u instanceof User
来源：http://wpt.hfpthk.cn

TS:   u instanceof User
来源：http://mvi.tianlin.xyz

Java: u instanceof User
来源：http://rev.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://lcg.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://wbo.hcnkem.com

C#:   u is User
来源：http://ofj.zdbjq.cn

[G14] 数据类 / record
来源：http://tfx.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jvu.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://aqc.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mna.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://lbs.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://yfe.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://fks.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lyo.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://sdr.jianghu66.top

[G15] 枚举
来源：http://pwl.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ebl.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ywb.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uaq.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eqp.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://wsu.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xie.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://dqq.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ggy.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://hct.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xvi.birdmap.top

PHP:  get_object_vars($obj);
来源：http://awy.shzxlz.cn

JS:   Object.entries(obj)
来源：http://kuu.aibaodan.cn

TS:   Object.entries(obj)
来源：http://gpb.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nal.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pkr.epnwcf.com

Ruby: obj.instance_variables
来源：http://pgc.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://jnz.ydzc1.top

================================================================================
来源：http://vmx.hcnkem.com

H. 异常与错误处理
来源：http://dqt.yvedp.cn

================================================================================
来源：http://wqo.hammf.cn

[H01] try / catch 基础
来源：http://bna.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lab.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hsd.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wwy.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fgq.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://luu.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wbd.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ziz.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fuv.xuanzx.com

[H02] finally / ensure 收尾
来源：http://qlt.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bhw.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mah.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iqp.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dda.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://txi.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pkm.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zqa.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://azn.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://kug.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://ksw.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://npe.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://dcj.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://zsq.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://osl.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jmw.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mux.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rzs.316326.xyz

[H04] 自定义异常类型
来源：http://phe.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://dao.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gqr.tian-w.cn

JS:   class MyError extends Error {}
来源：http://jkn.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://sxn.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://dcw.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gah.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://kib.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://ovl.shuidangran.top

[H05] 捕获特定类型
来源：http://pwo.svipenyu.cn

Py:   except ValueError as e:
来源：http://oob.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tci.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://iir.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://auc.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://oqz.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://joq.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://rkf.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dgc.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://sjm.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://pef.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://tge.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://paf.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ues.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qky.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://wnb.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://ktl.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://axj.hnqzz.top

[H07] 断言
来源：http://kvx.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://lhr.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://zzd.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://ala.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://wyq.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://zgd.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mzq.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://plj.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://tvd.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://otr.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://vvz.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pdw.jiagoushi.top

JS:   e.message;  e.stack
来源：http://fod.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://osq.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nju.ydjk.org.cn

Go:   err.Error()
来源：http://fca.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://wfm.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://xew.birdmap.top

[H09] 带错误码的异常
来源：http://yhn.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dlw.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://ces.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ivz.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tfk.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bic.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kxm.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ltn.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gjq.tarul.cn

[H10] 资源自动释放
来源：http://mnz.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gnp.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://trj.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nka.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://caf.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fxb.ivvv.top

Go:   defer f.Close()
来源：http://mna.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uvf.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://okw.ydjk.org.cn

================================================================================
来源：http://ktc.sysykeji.top

I. 正则表达式
来源：http://htz.xziqi.cn

================================================================================
来源：http://plr.zycfv.cn

[I01] 判断是否匹配
来源：http://vmt.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mem.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://hcb.yonumen.top

JS:   /\d+/.test(s)
来源：http://thf.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://erq.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tre.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ikn.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://bax.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vas.yuanzhike.top

[I02] 提取所有匹配
来源：http://jih.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://ovk.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hss.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ogs.tanke756.top

TS:   s.match(/\d+/g)
来源：http://wfv.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wwu.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://igo.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://fuv.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lxf.uphjek.com

[I03] 提取捕获分组
来源：http://ata.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ewb.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wms.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jhh.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ffi.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tba.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mcy.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ncy.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fnh.yangfankeji.com

[I04] 正则替换
来源：http://iav.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://tfr.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mbd.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://exr.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oql.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hqd.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cge.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lje.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kal.sjlbkw.cn

[I05] 按正则拆分
来源：http://lmm.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mal.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qvd.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://wjj.316326.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ueh.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://heq.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vgs.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ogk.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ont.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yng.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ily.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://etv.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lpl.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dtc.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zmp.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yfb.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ani.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kew.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://tmg.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fbq.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pgo.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qoq.jiagoushi.top

TS:   /error/gim
来源：http://rwf.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://abk.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fez.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://swd.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ppy.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://uxk.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vum.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cvu.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zvx.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nqd.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vbl.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mfs.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pug.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bjg.yonumen.top

================================================================================
来源：http://ias.feifeiyinyue.top

J. 日期与时间
来源：http://kfr.zhixingplan.top

================================================================================
来源：http://sar.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://rqo.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qew.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wvh.redwolf501.top

JS:   new Date();  Date.now()
来源：http://ipx.sweek.top

TS:   new Date();  Date.now()
来源：http://rop.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://hhi.yfazqb.com

Go:   time.Now()
来源：http://iud.yj20258.top

Ruby: Time.now
来源：http://mdu.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://icm.snrcjt.cn

[J02] 格式化输出
来源：http://sck.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://llm.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cmb.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rkq.jinqigufen.top

TS:   d.toISOString()
来源：http://usw.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dba.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dai.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yul.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xea.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://txb.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jel.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qio.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://jtm.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://qqy.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xbs.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pbq.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://zll.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://unj.wangdashe.top

[J04] 时间戳与日期互转
来源：http://ffu.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kxt.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bov.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ovq.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://hfk.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eel.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fnx.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kcw.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nxw.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://qdq.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://zij.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rmd.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dak.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xhy.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://mjr.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://imz.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://mnx.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://amv.haohaochexian.top

[J06] 计算两时间之差
来源：http://sjs.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://frb.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://kvl.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hqk.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vzq.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://oxu.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://rur.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://jeh.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://cys.316326.xyz

[J07] 比较两个日期
来源：http://wjn.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://ndw.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wtj.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://tit.gogol.net.cn


<!-- 参考信息 -->