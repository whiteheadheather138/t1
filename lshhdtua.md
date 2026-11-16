代发 wailian999

JS:   get name() { return this._name; }
来源：http://ldb.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://ipd.jqgfzy.top

Java: public String getName() { return name; }
来源：http://thy.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xbm.bbcook.cn

Ruby: attr_accessor :name
来源：http://bgt.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://egw.zhengqikj.top

[G12] 对象转字符串
来源：http://hwr.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://drx.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://brm.mhx1999.top

JS:   toString() { return this.name; }
来源：http://xdo.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://tqn.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://jst.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://uvs.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://prf.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://dej.sysykeji.top

[G13] 判断对象类型
来源：http://fuz.sysykeji.top

Py:   isinstance(u, User)
来源：http://rqh.fengsongda.top

PHP:  $u instanceof User
来源：http://fyp.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://zaf.hysaishi.cn

TS:   u instanceof User
来源：http://esu.cheryme.top

Java: u instanceof User
来源：http://uea.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://djs.yvedp.cn

Ruby: u.is_a?(User)
来源：http://dsf.quarkkingdee.top

C#:   u is User
来源：http://rrn.hammf.cn

[G14] 数据类 / record
来源：http://nif.gzhubu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bqx.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://jyv.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gia.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://pxb.sweek.top

Java: record User(String name, int age) {}
来源：http://uoo.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://htt.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sot.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://hxl.9152youxi.cn

[G15] 枚举
来源：http://xwr.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qaf.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://giq.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ovl.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ryo.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://lic.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yfp.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://zks.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qgq.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://vuc.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bgn.birdmap.top

PHP:  get_object_vars($obj);
来源：http://tqz.zhixingplan.top

JS:   Object.entries(obj)
来源：http://axt.xylfe.cn

TS:   Object.entries(obj)
来源：http://weo.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kwi.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dub.yuxming.cn

Ruby: obj.instance_variables
来源：http://diz.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://ncl.tarul.cn

================================================================================
来源：http://sro.birdmap.top

H. 异常与错误处理
来源：http://zwy.guannengcc.top

================================================================================
来源：http://prw.52xcode.cn

[H01] try / catch 基础
来源：http://xsd.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hpk.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jxx.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xia.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://flt.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sdo.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bit.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://icg.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mql.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://iay.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://pub.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fms.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tiw.zhaomingkeji.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://kkc.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://rnq.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nnu.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://woo.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://umv.xinyue.icu

[H03] 主动抛出异常
来源：http://lae.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://gap.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tdq.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://ztm.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://guc.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://olb.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cgr.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rob.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rfs.meibo888.top

[H04] 自定义异常类型
来源：http://uav.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://poh.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://djo.fktsv.cn

JS:   class MyError extends Error {}
来源：http://mol.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://srb.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://jdb.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nek.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://vxo.bbcook.cn

C#:   class MyException : Exception {}
来源：http://ncy.yangfankeji.com

[H05] 捕获特定类型
来源：http://apg.kuanghao11.cn

Py:   except ValueError as e:
来源：http://pov.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zvl.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://dkj.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://zge.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://xno.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rkh.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://amy.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iqe.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://zlk.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://zzk.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://bjz.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://kna.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vid.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://btc.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fsz.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://phc.zdbjq.cn

C#:   obj?.A?.B ?? default
来源：http://dlo.zycfv.cn

[H07] 断言
来源：http://hsw.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://ymd.ppjwa.cn

PHP:  assert($x > 0);
来源：http://nyq.yfazqb.com

JS:   console.assert(x > 0);
来源：http://vok.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://zue.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://jwj.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gcb.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://bej.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://dtm.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://ees.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://qyn.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ywo.cheryme.top

JS:   e.message;  e.stack
来源：http://djb.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pgk.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://bee.yvedp.cn

Go:   err.Error()
来源：http://rlq.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://ezr.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://bch.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://oiw.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mgu.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hxn.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lay.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ypm.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bxr.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eml.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://pdb.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hdg.xuetiantiany.cn

[H10] 资源自动释放
来源：http://lmm.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qwf.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://evn.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://avv.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yyi.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fnw.aibaodan.cn

Go:   defer f.Close()
来源：http://jev.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://exz.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kih.fehbvm.com

================================================================================
来源：http://ldb.52xcode.cn

I. 正则表达式
来源：http://vze.xinyue.icu

================================================================================
来源：http://uzl.quarkkingdee.top

[I01] 判断是否匹配
来源：http://mfb.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xfr.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://rzz.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://osy.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://gtj.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://exq.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kga.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://hfo.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://etd.hammf.cn

[I02] 提取所有匹配
来源：http://bki.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://lmb.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ugx.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kwf.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://geo.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://twn.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bnj.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://lxk.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gub.tarul.cn

[I03] 提取捕获分组
来源：http://ebg.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://udz.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uyy.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yvb.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tgg.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cks.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rex.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rnn.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ctb.quarkkingdee.top

[I04] 正则替换
来源：http://fot.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://njq.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://llc.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://tyg.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zff.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jrk.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://otv.zhongyouzk.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ffi.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wgt.yangfankeji.com

[I05] 按正则拆分
来源：http://wwz.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nll.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sad.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://bkz.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://awu.kuanghao11.cn

Java: s.split("\\s*,\\s*")
来源：http://abv.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hex.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rfc.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pwm.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dyg.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ffh.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qph.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rkm.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cmi.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vvy.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hgf.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rxa.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lhi.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://nih.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nmg.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://twf.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://buy.0kj1m.cn

TS:   /error/gim
来源：http://uyk.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ptl.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fzl.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://mcn.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://msr.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://jdw.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://agv.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nmw.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mbu.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxm.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jvz.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ojk.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mun.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jkx.ywan-chungtsiang.top

================================================================================
来源：http://hnt.sxryk.cn

J. 日期与时间
来源：http://mic.hfpthk.cn

================================================================================
来源：http://hmb.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://kuq.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yag.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pft.cashguo.top

JS:   new Date();  Date.now()
来源：http://lud.nwbrower.top

TS:   new Date();  Date.now()
来源：http://izp.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ctu.hesvh.cn

Go:   time.Now()
来源：http://abr.ivvv.top

Ruby: Time.now
来源：http://yqj.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://szs.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://dpo.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sbr.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rxv.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://glg.xinyue.icu

TS:   d.toISOString()
来源：http://cwy.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aib.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cpc.jyoumei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://css.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nfl.tian-w.cn

[J03] 字符串解析为日期
来源：http://aqa.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pzt.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hqs.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://qtw.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://mfo.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qyh.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sic.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://jiw.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wxu.fzhhl.top

[J04] 时间戳与日期互转
来源：http://nro.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fwd.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rmk.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uwo.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fzi.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pcj.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lyj.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pdj.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ket.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://vuj.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://bjd.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oox.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jsf.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvt.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://ysj.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zym.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://fur.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://bir.hnxiangtu.top

[J06] 计算两时间之差
来源：http://mtl.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://ezz.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://fww.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://whb.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wsj.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://igz.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://wnq.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://eae.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://vos.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://pln.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://izn.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zud.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://fxy.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://gnf.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pkw.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tlx.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kma.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://xys.hammf.cn

[J08] 提取年月日与星期
来源：http://lzx.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xfp.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mgg.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mli.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ksc.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://guc.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uca.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mqq.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kxm.sxryk.cn

[J09] 时区处理
来源：http://fgi.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vsr.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://woe.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cnp.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzo.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qxe.hfpthk.cn


<!-- 参考信息 -->