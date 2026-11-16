代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hst.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dnf.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://qxb.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://akl.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://aiv.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://fod.vehdjk.com

TS:   Object.entries(obj)
来源：http://fka.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cow.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://shq.yfazqb.com

Ruby: obj.instance_variables
来源：http://fxo.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://apt.yuxming.cn

================================================================================
来源：http://lvc.pycfn.com

H. 异常与错误处理
来源：http://sjh.zhengqikj.top

================================================================================
来源：http://zxo.xylfe.cn

[H01] try / catch 基础
来源：http://ebz.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zje.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sok.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ton.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfd.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mei.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qai.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hxt.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://adk.daria6918.cn

[H02] finally / ensure 收尾
来源：http://mwq.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jzi.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kye.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nvy.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nhw.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bro.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ndd.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://trw.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bnt.zhoulong.xyz

[H03] 主动抛出异常
来源：http://yet.sweek.top

Py:   raise ValueError("错误信息")
来源：http://upr.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lkp.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://iim.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://svy.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://wzb.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pne.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://avd.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://tfl.shuidangran.top

[H04] 自定义异常类型
来源：http://glz.tarul.cn

Py:   class MyError(Exception): pass
来源：http://wdp.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dlr.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://lag.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://ydj.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://cef.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tgo.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://enm.tian-w.cn

C#:   class MyException : Exception {}
来源：http://qqw.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://lwo.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://bed.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://joq.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://yio.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://voy.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://kot.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://usx.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://bga.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kga.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://wwp.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://ocl.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://lzl.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://eny.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://smu.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mig.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fny.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://kcy.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://ydj.shzxlz.cn

[H07] 断言
来源：http://tqe.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://jan.bjfxy.top

PHP:  assert($x > 0);
来源：http://rol.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://phj.yonumen.top

TS:   console.assert(x > 0);
来源：http://ckv.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://uja.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lse.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://phr.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://sta.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://jhk.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://zum.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kjd.sxryk.cn

JS:   e.message;  e.stack
来源：http://rvq.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qnw.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jih.zhongyouzk.top

Go:   err.Error()
来源：http://vmw.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://hsv.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://yex.cheryme.top

[H09] 带错误码的异常
来源：http://lrl.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bey.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://djx.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eqp.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qpe.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://irq.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dmz.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://qwb.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qll.yuxming.cn

[H10] 资源自动释放
来源：http://snh.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qlf.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hbi.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://smd.jinqigfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xie.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ong.0kj1m.cn

Go:   defer f.Close()
来源：http://pks.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dtf.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xwa.yj202588.top

================================================================================
来源：http://eko.hongshengwenyu.top

I. 正则表达式
来源：http://qyt.sweek.top

================================================================================
来源：http://bph.zhengqikj.top

[I01] 判断是否匹配
来源：http://pxu.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kih.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mhq.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://ghe.meibo888.top

TS:   /\d+/.test(s)
来源：http://uof.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gtg.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://axm.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://zju.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fdx.shuidangran.top

[I02] 提取所有匹配
来源：http://wrs.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://cui.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kvl.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jkq.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://rwp.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vgm.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sfy.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://poo.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gwl.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://itt.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aun.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nqg.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jhv.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ggv.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kit.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yid.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dxe.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tvi.pycfn.com

[I04] 正则替换
来源：http://wcc.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ibm.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wss.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://uum.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://ohc.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://pfr.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rob.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hbo.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qmn.pengpengdd.cyou

[I05] 按正则拆分
来源：http://ori.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vuu.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xkn.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://ftg.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://kdh.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://bpe.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tpl.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://lbv.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zmk.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yup.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://caz.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ceo.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lyn.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dyk.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://whe.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qzu.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dnn.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://meu.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://utc.ybcxt.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wbh.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xkz.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nmr.bbcook.cn

TS:   /error/gim
来源：http://xql.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lhk.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yjq.ybcxt.top

Ruby: s.scan(/error/i)
来源：http://uio.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jux.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://bmh.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aww.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qxm.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bji.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ath.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pdp.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yfc.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jts.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vzm.hysaishi.cn

================================================================================
来源：http://vha.zhiwuduotai.top

J. 日期与时间
来源：http://kmx.xuetiantiany.cn

================================================================================
来源：http://bbz.yj202588.top

[J01] 获取当前时间
来源：http://els.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fya.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oja.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://scw.hnqzz.top

TS:   new Date();  Date.now()
来源：http://fkj.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jgh.zhiwuduotai.top

Go:   time.Now()
来源：http://los.guowangkeji.top

Ruby: Time.now
来源：http://xdc.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rda.smart0.xyz

[J02] 格式化输出
来源：http://xyp.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vnf.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mhc.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ykm.svipenyu.cn

TS:   d.toISOString()
来源：http://vos.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mzy.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zyh.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssr.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://duc.c1oappe.top

[J03] 字符串解析为日期
来源：http://nal.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eyw.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fzk.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://gxt.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://wff.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://ypc.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qlz.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://fww.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hqt.havefunace.top

[J04] 时间戳与日期互转
来源：http://hab.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://viy.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jmg.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fix.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qbt.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://beh.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ang.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://klr.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uyo.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://kuv.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://dql.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tmt.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://smf.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pba.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://oha.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eah.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://lju.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://nze.shzxlz.cn

[J06] 计算两时间之差
来源：http://xgc.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://bvb.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://xkx.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gvp.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://xay.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://fnn.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://kes.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://ybu.kuanghao11.cn

[J07] 比较两个日期
来源：http://wyj.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://iqn.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bah.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://zeq.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wlg.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xcl.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lsb.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://iug.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://kaq.yueranfly.top

[J08] 提取年月日与星期
来源：http://rea.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vur.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wfd.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rdk.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kjf.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://afl.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yvk.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xdf.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ezb.chenlongwang.top

[J09] 时区处理
来源：http://jzw.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sjy.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ysy.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://svi.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ggz.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fqm.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kwm.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tzd.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xik.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://xfm.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jwb.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://plx.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yjn.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kln.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qok.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ktd.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jhv.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zwk.hammf.cn

================================================================================
来源：http://ngu.gzhubu.top

K. JSON 与序列化
来源：http://mxb.gaohongyu789.top

================================================================================
来源：http://yle.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://nnl.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qjv.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mme.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://ehc.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://vru.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qda.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://toz.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://dme.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pih.redwolf501.top

[K02] JSON 字符串转对象
来源：http://csd.chenzaomai.com

Py:   json.loads(s)
来源：http://xjb.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tsi.fzhhl.top

JS:   JSON.parse(s)
来源：http://jsj.jinqigufen.top

TS:   JSON.parse(s)
来源：http://epk.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://upb.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://peb.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://egz.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://avm.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://ywr.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bim.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xtw.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://llp.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tnv.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jes.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uek.dashuyun.cn


<!-- 参考信息 -->