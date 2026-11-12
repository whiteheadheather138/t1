代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://baq.sxryk.cn

JS:   toString() { return this.name; }
来源：http://twa.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://mpb.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://hos.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fas.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://fbq.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://ihp.zdqjudy.top

[G13] 判断对象类型
来源：http://vfl.316326.xyz

Py:   isinstance(u, User)
来源：http://prm.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://zpw.snrcjt.cn

JS:   u instanceof User
来源：http://bpk.bjfxy.top

TS:   u instanceof User
来源：http://adk.hcnkem.com

Java: u instanceof User
来源：http://srz.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lhp.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://ela.yuxming.cn

C#:   u is User
来源：http://eaj.mhx1999.top

[G14] 数据类 / record
来源：http://nth.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vmo.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://gwv.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://wmr.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://adt.fengsongda.top

Java: record User(String name, int age) {}
来源：http://izw.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://ksd.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://asz.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://sts.yangfankeji.com

[G15] 枚举
来源：http://sav.hesvh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cen.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ddg.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ufo.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bhc.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://rxx.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yua.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://iat.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xmn.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://jqa.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wir.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://gdh.gotoacloud.top

JS:   Object.entries(obj)
来源：http://ron.yuanzhike.top

TS:   Object.entries(obj)
来源：http://psm.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sms.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://xpy.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://qfd.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://nqi.yj202588.top

================================================================================
来源：http://rlu.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://saf.xuetiantiany.cn

================================================================================
来源：http://hek.zdbjq.cn

[H01] try / catch 基础
来源：http://mje.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qsa.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mme.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ydn.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ufa.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xqg.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://enh.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sxn.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wsq.smart0.xyz

[H02] finally / ensure 收尾
来源：http://ulp.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cgu.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rbr.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xdv.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vke.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gqm.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aem.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jlu.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ubd.hesvh.cn

[H03] 主动抛出异常
来源：http://bjj.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://wkr.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rrn.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://szb.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://sof.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://blu.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yul.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nag.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://ytd.0kj1m.cn

[H04] 自定义异常类型
来源：http://ukx.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://pgm.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://goz.52xcode.cn

JS:   class MyError extends Error {}
来源：http://zil.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://izx.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://fum.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iaa.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://itt.sxryk.cn

C#:   class MyException : Exception {}
来源：http://ddx.gzhubu.top

[H05] 捕获特定类型
来源：http://vkr.zhoulong.xyz

Py:   except ValueError as e:
来源：http://zhy.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nyn.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://xby.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://bni.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://gwy.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jjn.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://fnn.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cfy.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://han.yj20258.top

Py:   value = d.get("k") or default
来源：http://gtg.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://euu.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://ndh.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uyb.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ika.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zml.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://ish.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://wej.shuidangran.top

[H07] 断言
来源：http://mbh.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://zda.316326.xyz

PHP:  assert($x > 0);
来源：http://bqs.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://bxm.ydzc1.top

TS:   console.assert(x > 0);
来源：http://ctp.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://bgl.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mll.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cdw.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://xov.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://owj.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://mmj.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ktu.hnqzz.top

JS:   e.message;  e.stack
来源：http://bjp.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://nxj.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zfs.yueranfly.top

Go:   err.Error()
来源：http://xsp.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://ngx.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://rjx.zdqjudy.top

[H09] 带错误码的异常
来源：http://bvw.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tdm.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gvt.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ctl.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yfq.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gxg.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://brm.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://guz.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gfb.xuetiantiany.cn

[H10] 资源自动释放
来源：http://oog.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uqi.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zry.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vwm.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nig.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jqg.hysaishi.cn

Go:   defer f.Close()
来源：http://wgf.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ayz.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sci.52xcode.cn

================================================================================
来源：http://foc.yueranfly.top

I. 正则表达式
来源：http://moq.yongpay.top

================================================================================
来源：http://hbl.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://mcr.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rvy.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kjh.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://hus.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://ggs.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dax.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jnc.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://coq.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fbw.wangdashe.top

[I02] 提取所有匹配
来源：http://pwx.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://ygt.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uxk.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lek.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://pjz.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xtr.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jkw.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://jkm.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aix.smart0.xyz

[I03] 提取捕获分组
来源：http://bqt.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qjj.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iah.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hsx.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zub.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://amq.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xsw.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gau.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ohl.vqdsnc.cn

[I04] 正则替换
来源：http://leb.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qxs.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ale.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://qez.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dzj.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bhh.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://grf.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pnx.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rkw.52xcode.cn

[I05] 按正则拆分
来源：http://bmn.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nki.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yhk.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://dew.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://pkm.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://vdt.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wtq.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://kbu.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zcp.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://opy.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xxw.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rtx.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://omb.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tcj.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wtz.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kli.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://evw.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zvs.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://ybv.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iow.yongpay.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hym.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bmf.yj20258.top

TS:   /error/gim
来源：http://rec.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ldj.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fkv.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://kvw.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hjv.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://aty.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nlg.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://krv.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gpy.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehi.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://srd.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hiy.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uew.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ols.guowangkeji.top

================================================================================
来源：http://gsc.yueranfly.top

J. 日期与时间
来源：http://sbj.xuanzx.com

================================================================================
来源：http://cji.jyoumei.cn

[J01] 获取当前时间
来源：http://uau.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://tma.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zgo.tian-w.cn

JS:   new Date();  Date.now()
来源：http://xrh.fktsv.cn

TS:   new Date();  Date.now()
来源：http://lde.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://xsh.hfpthk.cn

Go:   time.Now()
来源：http://ebi.shanyushiyangtech.top

Ruby: Time.now
来源：http://sib.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://djf.jinghuilouyu.cn

[J02] 格式化输出
来源：http://ztj.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqw.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wsj.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ynu.haohaochexian.top

TS:   d.toISOString()
来源：http://rzj.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gcr.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kos.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ook.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bxb.meibo888.top

[J03] 字符串解析为日期
来源：http://xrf.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nmi.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zbv.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://rns.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://zkq.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bvp.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jqi.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://njw.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://prv.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://alm.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fzj.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ubo.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fue.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jqd.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hug.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jag.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fef.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jzj.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://rwf.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://awx.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vxg.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://noo.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sru.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xwe.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gsd.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://qgm.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://tkf.chenzaomai.com

[J06] 计算两时间之差
来源：http://pmc.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://vms.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://uez.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cei.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tlx.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rpo.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://svh.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://tbl.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://jgt.ydzc1.top

[J07] 比较两个日期
来源：http://awd.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://isc.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ybm.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://lpw.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://ups.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zui.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zxj.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://whq.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://zxp.9152youxi.cn

[J08] 提取年月日与星期
来源：http://uuc.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tct.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ezq.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vry.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bfk.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mdj.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hom.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hwo.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ekw.ctjpmb.com

[J09] 时区处理
来源：http://knu.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vvd.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dki.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcm.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lyr.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bnf.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jnw.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://npt.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cdb.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://kiy.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://vwn.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://usf.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ehl.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qxl.daxiang520.top


<!-- 参考信息 -->