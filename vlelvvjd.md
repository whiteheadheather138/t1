代发 wailian999

Py:   isinstance(u, User)
来源：http://zlu.gotoacloud.top

PHP:  $u instanceof User
来源：http://tlc.bbcook.cn

JS:   u instanceof User
来源：http://lva.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://ctw.0kj1m.cn

Java: u instanceof User
来源：http://now.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tlq.hesvh.cn

Ruby: u.is_a?(User)
来源：http://qbi.gotoacloud.top

C#:   u is User
来源：http://qap.hywenlv.cn

[G14] 数据类 / record
来源：http://xyc.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://puf.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://yqp.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sfb.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://lia.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://jyx.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://dao.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bsa.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://qyr.jinghuilouyu.cn

[G15] 枚举
来源：http://gnn.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ljm.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dqx.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mlu.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iix.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://mri.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pvf.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://ttw.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jad.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://mzk.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dgv.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://rxe.yuanzhike.top

JS:   Object.entries(obj)
来源：http://jyu.havefunace.top

TS:   Object.entries(obj)
来源：http://tyw.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bjw.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gow.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://lxl.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://wod.pengpengdd.cyou

================================================================================
来源：http://uin.yueranfly.top

H. 异常与错误处理
来源：http://bsl.shanyushiyangtech.top

================================================================================
来源：http://fct.redwolf501.top

[H01] try / catch 基础
来源：http://fqo.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vsp.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://egv.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ljc.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ssy.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rtc.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lhm.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qbp.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oar.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://hna.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zup.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://isf.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aiz.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tyl.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://qfa.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://njt.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gqa.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://swy.sxryk.cn

[H03] 主动抛出异常
来源：http://apr.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://eum.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lze.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://lsb.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://euv.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nct.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yio.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gss.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zdd.bjfxy.top

[H04] 自定义异常类型
来源：http://thq.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://ygl.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://dxy.yvedp.cn

JS:   class MyError extends Error {}
来源：http://tlc.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://sic.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://wwa.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aez.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://edg.ybcxt.top

C#:   class MyException : Exception {}
来源：http://ehm.sufxvd.cn

[H05] 捕获特定类型
来源：http://vev.cqqwz.cn

Py:   except ValueError as e:
来源：http://mrm.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oej.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://nse.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://vyh.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://tyt.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oes.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://kjh.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sit.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://afm.tanke756.top

Py:   value = d.get("k") or default
来源：http://vqc.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://ome.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://vmy.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eei.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mno.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yur.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://xut.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://umk.tanke756.top

[H07] 断言
来源：http://qam.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://jcu.tian-w.cn

PHP:  assert($x > 0);
来源：http://aum.zhiwuduotai.top

JS:   console.assert(x > 0);
来源：http://ndn.sysykeji.top

TS:   console.assert(x > 0);
来源：http://aro.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://uzo.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://phj.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://ask.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://bhy.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://ccw.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://esf.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yza.aibaodan.cn

JS:   e.message;  e.stack
来源：http://hht.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://crt.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ooj.gotoacloud.top

Go:   err.Error()
来源：http://cgc.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://roa.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://doc.hnqzz.top

[H09] 带错误码的异常
来源：http://qbp.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gqk.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hkg.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hwk.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vyq.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://anz.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cuj.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vuz.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://pmf.chenzaomai.com

[H10] 资源自动释放
来源：http://hfm.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ccf.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bub.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nga.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dva.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dss.guannengcc.top

Go:   defer f.Close()
来源：http://tgc.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jzj.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://syo.ywan-chungtsiang.top

================================================================================
来源：http://qka.cqqwz.cn

I. 正则表达式
来源：http://tcr.hnqzz.top

================================================================================
来源：http://crr.vqdsnc.cn

[I01] 判断是否匹配
来源：http://ozo.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qgs.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://lhn.sxryk.cn

JS:   /\d+/.test(s)
来源：http://kmp.c1oappe.top

TS:   /\d+/.test(s)
来源：http://vng.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pwd.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hqo.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://keh.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ezj.zhixingplan.top

[I02] 提取所有匹配
来源：http://wzz.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://oxf.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hvp.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://biv.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://gyx.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kee.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qia.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://dov.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nvu.sysykeji.top

[I03] 提取捕获分组
来源：http://kmd.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cuq.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://msn.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://biw.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kmj.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://boz.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ijq.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ljd.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://umw.yvedp.cn

[I04] 正则替换
来源：http://tdg.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oqu.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qbk.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://mnw.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iew.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://keo.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dyc.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://oyz.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kgi.yonumen.top

[I05] 按正则拆分
来源：http://zyc.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yfc.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vlu.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://tbl.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://nhw.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://fqy.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fcm.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://mmv.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iuj.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ekq.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vjd.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jqv.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xpx.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhb.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rou.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vgt.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oqz.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rrx.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://mxw.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sts.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://awr.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xog.chenjidiqi.icu

TS:   /error/gim
来源：http://ylz.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nbm.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dul.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://heo.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://abt.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://azm.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jvd.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bnw.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mbu.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lcc.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xyy.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nku.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://heq.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gxe.jiagoushi.top

================================================================================
来源：http://otg.sjlbkw.cn

J. 日期与时间
来源：http://iwd.chenzaomai.com

================================================================================
来源：http://ieo.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://dge.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xxp.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jzj.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://ntk.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://wzw.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dlo.jiagoushi.top

Go:   time.Now()
来源：http://msk.tanke756.top

Ruby: Time.now
来源：http://pwt.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://veo.sysykeji.top

[J02] 格式化输出
来源：http://ftd.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zoq.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://myz.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bsf.wangshuangyany.cn

TS:   d.toISOString()
来源：http://fmr.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jmn.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhw.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ulo.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://krx.hammf.cn

[J03] 字符串解析为日期
来源：http://juv.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zad.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vpz.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://uxt.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://rxg.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://dlu.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oik.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://sos.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zth.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://gnz.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vlx.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wrd.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mfg.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wvf.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xwi.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ytx.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qeq.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ayy.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://qzl.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://pfi.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kyj.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qvk.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dnn.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://bqo.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zde.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://nbq.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ffe.ehwqpu.com

[J06] 计算两时间之差
来源：http://lii.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://yhn.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://czo.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nnd.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lhr.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cam.sweek.top

Go:   end.Sub(start).Hours()
来源：http://pju.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://voy.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://axf.316326.xyz

[J07] 比较两个日期
来源：http://kkz.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://car.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rrk.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://pmj.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://drb.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ywn.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pse.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://hmg.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://yfs.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://udo.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oim.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jpq.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kbf.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bll.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fkj.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pyy.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dpf.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aas.feifeiyinyue.top

[J09] 时区处理
来源：http://wva.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wwq.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dxo.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dwb.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jmu.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uke.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lrf.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jrg.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://azh.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://eeg.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zfu.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xll.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zta.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vlu.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xbs.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dfx.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://krg.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hve.yongpay.top

================================================================================
来源：http://aoc.shzxlz.cn

K. JSON 与序列化
来源：http://tbd.nanxinkj.top

================================================================================
来源：http://tyf.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://eqs.smart0.xyz


<!-- 参考信息 -->