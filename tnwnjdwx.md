代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://cwv.hcnkem.com

Java: record User(String name, int age) {}
来源：http://ozi.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://nkj.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tpq.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://kwu.hongshengwenyu.top

[G15] 枚举
来源：http://ifp.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uek.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wlw.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nmx.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ppa.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://kio.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bzz.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://oql.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://igi.smart0.xyz

[G16] 对象转数组 / 字典
来源：http://ccr.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cwp.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://zcq.zdbjq.cn

JS:   Object.entries(obj)
来源：http://hrs.shuidangran.top

TS:   Object.entries(obj)
来源：http://hzz.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ndp.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pto.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://tmx.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://lip.xinyue.icu

================================================================================
来源：http://hrr.hammf.cn

H. 异常与错误处理
来源：http://gnd.zhijiandao.cn

================================================================================
来源：http://qon.andypj.xyz

[H01] try / catch 基础
来源：http://mdx.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zwf.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aar.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qca.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://upv.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fbs.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pir.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ick.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sue.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://fpi.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://sgo.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mzm.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uqf.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vuv.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://ajq.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ulf.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bcf.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cbn.cashguo.top

[H03] 主动抛出异常
来源：http://thu.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://yma.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fzm.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://iha.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://zql.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ucr.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://obc.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tur.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://sxf.andypj.xyz

[H04] 自定义异常类型
来源：http://xwb.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://lqu.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pil.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://gvi.daria6918.cn

TS:   class MyError extends Error {}
来源：http://etc.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://thv.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ybt.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://srq.sxryk.cn

C#:   class MyException : Exception {}
来源：http://eff.cheryme.top

[H05] 捕获特定类型
来源：http://too.jyoumei.cn

Py:   except ValueError as e:
来源：http://gcq.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uoy.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://izi.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://hod.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://akr.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cib.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://wud.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tej.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://nmb.cucudq.cn

Py:   value = d.get("k") or default
来源：http://tmi.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://xmk.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hca.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oxl.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mtr.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gxh.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://hcf.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://ryb.jinqigfzy.top

[H07] 断言
来源：http://qtn.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://xut.zhengqikj.top

PHP:  assert($x > 0);
来源：http://xxa.fehbvm.com

JS:   console.assert(x > 0);
来源：http://bqp.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://vua.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://ikn.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ykb.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mea.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://bgs.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://icn.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://sno.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wcr.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://jfg.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://pcl.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://emd.52xcode.cn

Go:   err.Error()
来源：http://mji.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://khs.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://sly.fzhhl.top

[H09] 带错误码的异常
来源：http://nwf.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iur.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rph.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://acu.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ptu.andypj.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bvy.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hwe.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://foh.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nll.ydzc1.top

[H10] 资源自动释放
来源：http://geq.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fxh.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://chb.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zar.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nop.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xdt.jianghu66.top

Go:   defer f.Close()
来源：http://nvq.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dfb.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bjp.sufxvd.cn

================================================================================
来源：http://uni.haohaochexian.top

I. 正则表达式
来源：http://uen.smart0.xyz

================================================================================
来源：http://pxt.52xcode.cn

[I01] 判断是否匹配
来源：http://pcl.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nek.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://blv.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://wlc.sysykeji.top

TS:   /\d+/.test(s)
来源：http://lkf.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://anj.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vmy.hcnkem.com

Ruby: s.match?(/\d+/)
来源：http://zpz.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zmz.guowangkeji.top

[I02] 提取所有匹配
来源：http://rlj.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://jby.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://grx.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mjb.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://hxs.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hof.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zxe.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://fep.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yfm.jqgfzy.top

[I03] 提取捕获分组
来源：http://gku.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://edr.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rbk.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nco.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://arm.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wrv.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qaj.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://exj.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://spt.hesvh.cn

[I04] 正则替换
来源：http://vjq.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fdn.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uqc.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://upg.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://vwh.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://ypg.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://svv.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ikv.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lel.chenlongwang.top

[I05] 按正则拆分
来源：http://fps.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://epn.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jov.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://isp.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://ywj.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://qch.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cnv.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://umk.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mop.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ula.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cwf.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://laj.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lse.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxe.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lvk.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qkg.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fmr.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fbs.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://cfq.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yug.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ovs.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kio.chenjidiqi.icu

TS:   /error/gim
来源：http://php.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://btn.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dlf.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://yhy.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pwx.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://fze.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mgz.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ogx.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sgd.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://okz.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cty.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vse.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://muh.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kvi.sxryk.cn

================================================================================
来源：http://ily.fehbvm.com

J. 日期与时间
来源：http://zgn.chenzaomai.com

================================================================================
来源：http://tyr.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://tds.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jqv.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yhr.yonumen.top

JS:   new Date();  Date.now()
来源：http://gmj.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://nij.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wbk.zhoulong.xyz

Go:   time.Now()
来源：http://ohy.andypj.xyz

Ruby: Time.now
来源：http://jtq.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bks.jqgfzy.top

[J02] 格式化输出
来源：http://mvb.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rkl.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cms.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bmo.zhoulong.xyz

TS:   d.toISOString()
来源：http://uau.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://any.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgf.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vsi.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mla.smart0.xyz

[J03] 字符串解析为日期
来源：http://zcl.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xii.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://snl.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://plc.tarul.cn

TS:   new Date("2024-01-02")
来源：http://bbn.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ifq.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ams.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://frf.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ipq.yj20258888.top

[J04] 时间戳与日期互转
来源：http://dzo.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ufj.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ttg.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eia.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://sos.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hjv.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eso.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uoy.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://llw.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://nfu.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://fxk.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kdb.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jyt.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aun.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://ilz.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://brk.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://eya.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bsm.hywenlv.cn

[J06] 计算两时间之差
来源：http://jpb.meibo888.top

Py:   (end - start).total_seconds()
来源：http://cux.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://zgm.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mmr.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tbo.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://zuv.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://zwt.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://obh.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://nnm.hammf.cn

[J07] 比较两个日期
来源：http://onf.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://axq.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gmu.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vvj.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mmy.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://spj.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rjp.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://yrt.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://jcu.ydzc1.top

[J08] 提取年月日与星期
来源：http://abx.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sjn.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vme.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://onu.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aih.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oto.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lyq.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ykg.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qrf.dianchejie.cn

[J09] 时区处理
来源：http://hxd.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baf.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zxa.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qvz.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wup.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kyp.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qvu.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wld.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gtm.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://fkx.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ony.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://emr.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nkd.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ghl.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xyd.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://acq.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hea.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fka.zhaomingkeji.xyz

================================================================================
来源：http://dbj.zhijiandao.cn

K. JSON 与序列化
来源：http://log.hywenlv.cn

================================================================================
来源：http://jns.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://jgm.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sdl.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yyy.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://abu.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://eak.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dgg.fehbvm.com

Go:   json.Marshal(obj)
来源：http://bvs.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ypu.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://skq.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://ytr.vehdjk.com

Py:   json.loads(s)
来源：http://qks.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lfx.hysaishi.cn

JS:   JSON.parse(s)
来源：http://num.pycfn.com


<!-- 参考信息 -->