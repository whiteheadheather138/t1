代发 wailian999

C#:   public / protected / private / internal
来源：http://vor.yuanzhike.top

[G11] getter / setter
来源：http://itw.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://qrw.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rzr.hcnkem.com

JS:   get name() { return this._name; }
来源：http://yhw.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://wit.snrcjt.cn

Java: public String getName() { return name; }
来源：http://gtn.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wcj.hcnkem.com

Ruby: attr_accessor :name
来源：http://vxc.cashguo.top

C#:   public string Name { get; set; }
来源：http://bep.316326.xyz

[G12] 对象转字符串
来源：http://dar.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://zje.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bbo.yonumen.top

JS:   toString() { return this.name; }
来源：http://nzg.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://ziv.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://koq.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xpm.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://lsf.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://hjf.yonumen.top

[G13] 判断对象类型
来源：http://apx.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://cyr.aizwys.cn

PHP:  $u instanceof User
来源：http://mmr.shangyingyoupin.top

JS:   u instanceof User
来源：http://jeh.iojbl.cn

TS:   u instanceof User
来源：http://pvr.bbcook.cn

Java: u instanceof User
来源：http://lkg.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vgn.xziqi.cn

Ruby: u.is_a?(User)
来源：http://sqs.yueranfly.top

C#:   u is User
来源：http://baw.yuxming.cn

[G14] 数据类 / record
来源：http://jwd.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yyq.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://mkv.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://ors.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://pfx.daxiang520.top

Java: record User(String name, int age) {}
来源：http://hki.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://ntx.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zsu.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://wzn.cdnleiting.top

[G15] 枚举
来源：http://ctp.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jys.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zvs.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ajc.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://izc.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://vxf.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vdn.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://srn.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fpi.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://rrk.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tmc.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://anh.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://axv.tarul.cn

TS:   Object.entries(obj)
来源：http://nhv.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sfq.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wuy.yj202588.top

Ruby: obj.instance_variables
来源：http://qkm.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://qyc.xuetiantiany.cn

================================================================================
来源：http://mua.tanke756.top

H. 异常与错误处理
来源：http://qhv.hywenlv.cn

================================================================================
来源：http://oym.tianlin.xyz

[H01] try / catch 基础
来源：http://nxt.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uzj.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fmn.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yjx.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qwn.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mjk.aizwys.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mbm.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rab.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cml.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://ogl.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://lij.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://exo.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hyx.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://fqn.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://akl.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yzb.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hkc.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aqg.yuanzhike.top

[H03] 主动抛出异常
来源：http://qtz.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://zln.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bgt.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://pma.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://bdr.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lgr.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ccg.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dpp.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fdw.hnxiangtu.top

[H04] 自定义异常类型
来源：http://fsa.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://eai.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://lrh.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://wdj.shuidangran.top

TS:   class MyError extends Error {}
来源：http://bbw.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://vqu.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://evc.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://ulo.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://osz.meibo888.top

[H05] 捕获特定类型
来源：http://mlu.fengsongda.top

Py:   except ValueError as e:
来源：http://hqa.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wdz.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://gsc.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://ngb.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://qva.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wkb.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://ppr.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bje.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://zkc.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://hgz.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://iuf.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dnu.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ebt.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zxr.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vnv.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://eik.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://cwv.zhongyouzk.top

[H07] 断言
来源：http://rkp.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://skv.zdqjudy.top

PHP:  assert($x > 0);
来源：http://dsq.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://las.smart0.xyz

TS:   console.assert(x > 0);
来源：http://uay.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://bit.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nwt.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uyo.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://quw.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://mev.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://tfi.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zuz.yfazqb.com

JS:   e.message;  e.stack
来源：http://gzf.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nat.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://goz.zhengqikj.top

Go:   err.Error()
来源：http://ggd.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://wwz.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://hlz.jqgufenzy.top

[H09] 带错误码的异常
来源：http://nmy.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oyo.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dmm.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hct.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ovc.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fqk.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wax.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://rjt.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tzs.redwolf501.top

[H10] 资源自动释放
来源：http://cgr.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zzf.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ccg.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qiz.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://htr.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xtr.hysaishi.cn

Go:   defer f.Close()
来源：http://qee.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://naz.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eer.mhx1999.top

================================================================================
来源：http://ckk.hnxiangtu.top

I. 正则表达式
来源：http://phi.ppjwa.cn

================================================================================
来源：http://ubq.tanke756.top

[I01] 判断是否匹配
来源：http://ild.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xae.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://vgi.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://qtl.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://wij.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://srt.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gmt.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://pyl.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://int.zhoulong.xyz

[I02] 提取所有匹配
来源：http://rin.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://gok.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wgn.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://drb.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://gfq.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pmh.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ghf.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://uvu.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://woq.vehdjk.com

[I03] 提取捕获分组
来源：http://xvc.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jsp.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lga.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iym.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vdd.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fga.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vbm.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wyh.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bta.wangdashe.top

[I04] 正则替换
来源：http://yxc.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jqz.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ouo.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uyx.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://waj.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://qal.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qyg.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kzr.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vbd.uphjek.com

[I05] 按正则拆分
来源：http://qlo.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aqi.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fhu.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://vwq.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://ovk.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://uij.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ecj.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://hlq.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kuw.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://txv.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdp.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jji.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qik.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yzk.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gol.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wyv.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iko.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tpl.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://cmf.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qrf.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://maf.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uua.ehwqpu.com

TS:   /error/gim
来源：http://qng.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://syf.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qei.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://bpm.andypj.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hcj.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://vnc.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bwa.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ttk.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ohw.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://geb.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wyp.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mee.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jdi.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uyc.ydzc1.top

================================================================================
来源：http://rfg.ybcxt.top

J. 日期与时间
来源：http://tqp.yj20258.top

================================================================================
来源：http://gkm.yangfankeji.com

[J01] 获取当前时间
来源：http://rky.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uow.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uca.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://aay.daxiang520.top

TS:   new Date();  Date.now()
来源：http://kdq.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rje.ppjwa.cn

Go:   time.Now()
来源：http://ntl.meibo888.top

Ruby: Time.now
来源：http://nlp.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zev.xuanzx.com

[J02] 格式化输出
来源：http://viw.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ibk.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ysj.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wrl.hfpthk.cn

TS:   d.toISOString()
来源：http://mwa.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dxi.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hqt.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hzj.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jmj.pycfn.com

[J03] 字符串解析为日期
来源：http://vpe.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yky.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lud.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://qvi.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://wvu.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://orl.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aeb.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://wcd.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bod.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://yxg.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wwf.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xkt.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xua.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dvc.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mmk.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kjg.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hao.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ozq.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://zud.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://vsd.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mox.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xnv.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lnq.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://qsf.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qav.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://acq.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://csj.ydjk.org.cn

[J06] 计算两时间之差
来源：http://pmv.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://cef.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://ill.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://znb.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wnj.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://znw.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://pwq.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://mgc.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://ofh.jqgfzy.top

[J07] 比较两个日期
来源：http://ohp.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://hbb.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qor.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://yih.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://uca.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vrc.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://csx.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://osq.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://izu.zycfv.cn

[J08] 提取年月日与星期
来源：http://djy.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eyu.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qce.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nei.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://owe.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eed.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ohb.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sub.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dfc.cucudq.cn

[J09] 时区处理
来源：http://hza.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mro.fktsv.cn


<!-- 参考信息 -->