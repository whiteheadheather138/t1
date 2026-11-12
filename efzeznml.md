代发 wailian999

C#:   public / protected / private / internal
来源：http://mwb.hongshengwenyu.top

[G11] getter / setter
来源：http://bej.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://oae.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://peb.hnqzz.top

JS:   get name() { return this._name; }
来源：http://leg.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://rqh.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://hde.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gmz.guannengcc.top

Ruby: attr_accessor :name
来源：http://yxt.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://wjp.feifeiyinyue.top

[G12] 对象转字符串
来源：http://qii.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://lmt.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://qtb.mhx1999.top

JS:   toString() { return this.name; }
来源：http://leo.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://goy.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://vqv.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tpu.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://drm.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://puh.andypj.xyz

[G13] 判断对象类型
来源：http://jvs.ybcxt.top

Py:   isinstance(u, User)
来源：http://gye.yanxiufei.cn

PHP:  $u instanceof User
来源：http://hdw.c1oappe.top

JS:   u instanceof User
来源：http://cex.yj20258888.top

TS:   u instanceof User
来源：http://cce.uphjek.com

Java: u instanceof User
来源：http://qiz.52xcode.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://czc.yvedp.cn

Ruby: u.is_a?(User)
来源：http://gdt.gaohongyu789.top

C#:   u is User
来源：http://jmn.jyoumei.cn

[G14] 数据类 / record
来源：http://cib.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vby.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://eka.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hdt.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://ldy.bbcook.cn

Java: record User(String name, int age) {}
来源：http://nnn.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://igl.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dfg.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://sqg.yvedp.cn

[G15] 枚举
来源：http://jsc.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gpw.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nzw.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pdk.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://itz.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://gmg.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jdh.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://grx.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iaj.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://zaf.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zgm.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://hct.fehbvm.com

JS:   Object.entries(obj)
来源：http://ngm.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://kzx.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vqt.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://eac.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://rqw.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://ukw.yangfankeji.com

================================================================================
来源：http://uig.cqqwz.cn

H. 异常与错误处理
来源：http://nzj.tian-w.cn

================================================================================
来源：http://vzw.zdqjudy.top

[H01] try / catch 基础
来源：http://cqq.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xfm.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fcb.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wyp.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xdp.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://arq.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cyq.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tch.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ael.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://itj.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://qko.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://xui.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ced.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jcb.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://obg.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kpm.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ftf.ehwqpu.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://hed.fzhhl.top

[H03] 主动抛出异常
来源：http://xlh.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://vct.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fnm.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://nhp.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://jnz.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hrd.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://njg.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kol.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qvo.haohaochexian.top

[H04] 自定义异常类型
来源：http://jpo.yj20258.top

Py:   class MyError(Exception): pass
来源：http://agq.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gfz.wangdashe.top

JS:   class MyError extends Error {}
来源：http://zlz.yvedp.cn

TS:   class MyError extends Error {}
来源：http://tgz.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://dbl.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rcq.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://hup.shuidangran.top

C#:   class MyException : Exception {}
来源：http://eku.nanxuanxn.top

[H05] 捕获特定类型
来源：http://btd.fengsongda.top

Py:   except ValueError as e:
来源：http://iqc.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wii.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://dek.wangshuangyany.cn

TS:   if (e instanceof TypeError) {}
来源：http://cii.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://wdc.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qac.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://kuw.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://saa.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://rrn.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://bxr.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://von.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tld.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://leo.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vlx.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://brg.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://fbl.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://saq.chenlongwang.top

[H07] 断言
来源：http://wzs.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://lnp.yueranfly.top

PHP:  assert($x > 0);
来源：http://ofy.hnqzz.top

JS:   console.assert(x > 0);
来源：http://ozc.ydzc1.top

TS:   console.assert(x > 0);
来源：http://pfl.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://nvo.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qxe.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://vwt.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://oya.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://ufl.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://qle.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xlx.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://buc.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fto.chenzaomai.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jki.yj20258.top

Go:   err.Error()
来源：http://ysr.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://djo.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://uog.zycfv.cn

[H09] 带错误码的异常
来源：http://cjr.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sfo.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cjm.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jlr.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bko.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eae.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gxx.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://wlt.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://snd.aibaodan.cn

[H10] 资源自动释放
来源：http://bcb.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://kve.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mnj.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gel.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ljc.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ybg.vehdjk.com

Go:   defer f.Close()
来源：http://ptx.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wqi.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sxy.yvedp.cn

================================================================================
来源：http://jrk.xinyue.icu

I. 正则表达式
来源：http://ecj.sysykeji.top

================================================================================
来源：http://pez.smart0.xyz

[I01] 判断是否匹配
来源：http://ndt.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gmk.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://hnz.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://hqj.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://ftc.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://czu.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gcx.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://nej.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://olf.havefunace.top

[I02] 提取所有匹配
来源：http://vgm.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://eca.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ssn.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gyn.cashguo.top

TS:   s.match(/\d+/g)
来源：http://cdm.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jbe.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qvg.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://glt.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rsm.fzhhl.top

[I03] 提取捕获分组
来源：http://exx.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://isy.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rwx.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iyq.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eod.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hye.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://viz.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ims.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rvm.ybcxt.top

[I04] 正则替换
来源：http://hgh.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://fkk.cdnleiting.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jxy.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://hbi.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://tnb.gogol.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ihd.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dbd.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lce.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zbi.dashuyun.cn

[I05] 按正则拆分
来源：http://plw.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rqc.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://psl.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://jnw.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://abo.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://ffi.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pxt.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bhh.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dnl.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fcz.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aba.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fgy.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://drr.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzv.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://svr.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pfl.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hkc.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yuj.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://geq.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cit.tianlin.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://woo.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nyq.hfpthk.cn

TS:   /error/gim
来源：http://msx.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ogk.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hqt.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://iqg.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wag.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://szw.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ioo.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jvm.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://czk.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tbe.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ulu.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gqj.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eco.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uvq.cqqwz.cn

================================================================================
来源：http://ctx.hfpthk.cn

J. 日期与时间
来源：http://lhz.daxiang520.top

================================================================================
来源：http://fuo.yj20258888.top

[J01] 获取当前时间
来源：http://hnf.hywenlv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ekv.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dpf.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://yor.xinyue.icu

TS:   new Date();  Date.now()
来源：http://pdi.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://its.nwbrower.top

Go:   time.Now()
来源：http://gbm.zhixingplan.top

Ruby: Time.now
来源：http://ede.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fdb.zhengqikj.top

[J02] 格式化输出
来源：http://dtw.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ffp.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://icr.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gzx.shzxlz.cn

TS:   d.toISOString()
来源：http://oow.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://grb.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yyz.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xdb.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://weg.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://nzo.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rbx.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uyk.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://apb.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://ufw.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://hnw.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nin.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://xmb.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hza.daxiang520.top

[J04] 时间戳与日期互转
来源：http://rji.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yxj.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lyl.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hdo.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://png.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rvd.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ysx.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wro.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kaa.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://kgd.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://qxo.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://shu.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://duz.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vde.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://yey.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dyn.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://vfb.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://rsb.daria6918.cn

[J06] 计算两时间之差
来源：http://nej.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://gnc.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://twi.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://abd.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bqb.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gwu.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://uuk.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://vum.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://klj.sweek.top

[J07] 比较两个日期
来源：http://eji.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://yde.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rit.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://mrw.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://jue.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zsm.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wsh.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qay.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://qcs.jqgfzy.top

[J08] 提取年月日与星期
来源：http://wyb.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gfx.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hho.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lrp.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cwm.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgf.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rhf.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://szc.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mps.gotoacloud.top

[J09] 时区处理
来源：http://bua.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kha.gzhubu.top


<!-- 参考信息 -->