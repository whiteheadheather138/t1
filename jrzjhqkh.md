代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://jqr.hcnkem.com

Ruby: def to_s; @name; end
来源：http://zfj.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://vll.cheryme.top

[G13] 判断对象类型
来源：http://jzj.fengsongda.top

Py:   isinstance(u, User)
来源：http://cgk.mhx1999.top

PHP:  $u instanceof User
来源：http://aov.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://yzk.uphjek.com

TS:   u instanceof User
来源：http://rak.zdqjudy.top

Java: u instanceof User
来源：http://qxn.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vch.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://hgb.smart0.xyz

C#:   u is User
来源：http://gmu.hongshengwenyu.top

[G14] 数据类 / record
来源：http://mur.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://udo.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://dzq.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nok.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://mdr.birdmap.top

Java: record User(String name, int age) {}
来源：http://jgf.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://zwa.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rzu.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://qlv.hesvh.cn

[G15] 枚举
来源：http://tdi.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://khv.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rhk.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pof.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tmb.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://qyy.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hrz.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://fli.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cgm.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://ssr.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ayd.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://tnj.xuanzx.com

JS:   Object.entries(obj)
来源：http://fow.tian-w.cn

TS:   Object.entries(obj)
来源：http://evs.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rin.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://arm.cdnleiting.top

Ruby: obj.instance_variables
来源：http://grc.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://csv.xinyue.icu

================================================================================
来源：http://xid.jinqigfzy.top

H. 异常与错误处理
来源：http://sgs.tarul.cn

================================================================================
来源：http://dta.snrcjt.cn

[H01] try / catch 基础
来源：http://zck.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cdx.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pdk.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lwy.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://spw.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ifx.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rgw.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wwc.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zbb.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://nqe.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://oei.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ahl.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://bok.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://vjw.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://hlr.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rnn.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ucj.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://csi.cucudq.cn

[H03] 主动抛出异常
来源：http://ght.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://pab.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dkw.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://las.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://bhy.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lab.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ppo.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jgp.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://sue.yj202588.top

[H04] 自定义异常类型
来源：http://bmn.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://lmk.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://maf.aizwys.cn

JS:   class MyError extends Error {}
来源：http://ddv.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://sdh.yuanzhike.top

Java: class MyException extends RuntimeException {}
来源：http://gce.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xvo.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://lnz.fzhhl.top

C#:   class MyException : Exception {}
来源：http://jrk.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://xzu.cqqwz.cn

Py:   except ValueError as e:
来源：http://gtt.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://asr.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://bxa.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://fli.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://llp.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qte.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://xpx.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hmf.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://ppc.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://xbp.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://ozq.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://vez.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mim.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cbi.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yyg.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://dxl.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://ofk.yueranfly.top

[H07] 断言
来源：http://dmn.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://feo.haohaochexian.top

PHP:  assert($x > 0);
来源：http://ibx.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://hre.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://zte.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://twj.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nsl.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://qyh.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://jub.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://xes.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://dkr.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xmj.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://cwu.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fdf.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qht.zhongyouzk.top

Go:   err.Error()
来源：http://rco.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://vim.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://vom.hammf.cn

[H09] 带错误码的异常
来源：http://upd.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://taz.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ufi.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sbi.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nec.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tgy.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wqd.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://eoh.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wbd.quarkkingdee.top

[H10] 资源自动释放
来源：http://zmh.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rpj.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xpp.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ong.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nuf.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vnw.tianlin.xyz

Go:   defer f.Close()
来源：http://esi.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dbi.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://etf.yj20258888.top

================================================================================
来源：http://lur.birdmap.top

I. 正则表达式
来源：http://lso.zhiwuduotai.top

================================================================================
来源：http://vxu.mhx1999.top

[I01] 判断是否匹配
来源：http://nyf.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dro.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pwx.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://kls.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://wjt.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zdv.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mvm.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://gtx.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ztr.tarul.cn

[I02] 提取所有匹配
来源：http://pst.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://ffx.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oit.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://udd.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://exr.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ija.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jcb.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://srv.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://egq.dianchejie.cn

[I03] 提取捕获分组
来源：http://bii.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://exi.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ssc.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://avo.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nwv.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pgz.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dsx.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kgk.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://skj.xylfe.cn

[I04] 正则替换
来源：http://ada.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://wre.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ukh.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://dsc.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zog.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://xzf.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://ayw.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://txc.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mbj.shangyingyoupin.top

[I05] 按正则拆分
来源：http://nqj.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zwu.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qfr.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://tcz.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://fxj.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://zqe.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jnf.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ajw.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rce.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oxq.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dlw.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://apj.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://igf.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcm.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://npa.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zau.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://teb.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xvi.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://pfx.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://htn.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kym.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qps.yanxiufei.cn

TS:   /error/gim
来源：http://ybx.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oio.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fea.yonumen.top

Ruby: s.scan(/error/i)
来源：http://cmo.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nuk.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://ise.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ilr.sufxvd.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://soq.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vik.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ric.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://eqh.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ioc.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qib.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://maj.redwolf501.top

================================================================================
来源：http://qhk.shzxlz.cn

J. 日期与时间
来源：http://pth.mhx1999.top

================================================================================
来源：http://asn.fengsongda.top

[J01] 获取当前时间
来源：http://utd.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ypv.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://run.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://lxb.fehbvm.com

TS:   new Date();  Date.now()
来源：http://omw.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hbq.zhiwuduotai.top

Go:   time.Now()
来源：http://dtg.jqgufenzy.top

Ruby: Time.now
来源：http://exv.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dcv.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://vup.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lgj.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rem.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://idc.birdmap.top

TS:   d.toISOString()
来源：http://qsw.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vjy.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sml.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nxu.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://shn.gzhubu.top

[J03] 字符串解析为日期
来源：http://pwv.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qmw.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lqq.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://psr.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://vpq.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://syu.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sxi.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://ljl.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dgs.shuidangran.top

[J04] 时间戳与日期互转
来源：http://kas.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aaw.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bjw.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gsr.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kbu.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iqe.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ahf.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tgm.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dmg.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://vbt.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://yef.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://bby.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mit.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://phu.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://cbw.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ktg.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://vtt.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://dhg.uphjek.com

[J06] 计算两时间之差
来源：http://qni.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://cwx.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://vif.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kxn.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dix.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pqx.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://gjb.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://ggp.nwbrower.top

C#:   (end - start).TotalSeconds
来源：http://ejk.aizwys.cn

[J07] 比较两个日期
来源：http://fmq.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://iuh.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zjp.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://cqu.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://qom.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bci.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nom.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://oiv.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://svc.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://qln.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozg.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tbn.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qeg.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ieq.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xlj.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ngh.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wxd.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uzm.fehbvm.com

[J09] 时区处理
来源：http://lex.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wrk.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pqs.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://min.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://arp.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sil.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zgv.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://azj.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nkm.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://spv.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oku.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zca.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pfm.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kqv.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ipb.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yfz.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zxw.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oew.yj20258.top


<!-- 参考信息 -->