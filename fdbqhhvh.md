代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://wot.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ydv.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://izb.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ciy.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://nkb.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://tum.xinyue.icu

TS:   Object.entries(obj)
来源：http://dkp.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pzx.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tap.haohaochexian.top

Ruby: obj.instance_variables
来源：http://auf.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://zge.daria6918.cn

================================================================================
来源：http://ktn.tarul.cn

H. 异常与错误处理
来源：http://dks.feifeiyinyue.top

================================================================================
来源：http://rwl.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://amh.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nif.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lha.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gno.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jhg.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bqa.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hvk.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uuq.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xfn.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://jjd.fehbvm.com

Py:   try: f()⏎finally: cleanup()
来源：http://ddj.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ioi.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vfr.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://khc.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://dtk.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://mpf.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://isu.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://yxn.ehwqpu.com

[H03] 主动抛出异常
来源：http://wto.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://dyx.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dtv.tanke756.top

JS:   throw new Error("错误信息");
来源：http://sth.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://fec.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gzo.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vxu.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ykz.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://vry.316326.xyz

[H04] 自定义异常类型
来源：http://cre.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://vrm.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://hpe.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://zgo.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://udz.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://bxc.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bfu.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://tvj.52xcode.cn

C#:   class MyException : Exception {}
来源：http://qyz.yvedp.cn

[H05] 捕获特定类型
来源：http://zmq.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://rrb.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bwq.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://knk.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://ngb.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://cdi.cdnleiting.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lfv.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://vxl.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://etw.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://nct.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://oad.bjfxy.top

PHP:  $v = $d["k"] ?? null;
来源：http://xwc.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ptf.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://hcn.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://out.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://amc.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://iki.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://dhu.smart0.xyz

[H07] 断言
来源：http://lqu.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://kgl.havefunace.top

PHP:  assert($x > 0);
来源：http://lix.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://drn.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://djc.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://omd.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uph.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ovj.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://mpe.sweek.top

[H08] 获取错误信息与堆栈
来源：http://lhb.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://mho.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kzc.pycfn.com

JS:   e.message;  e.stack
来源：http://ynp.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vxv.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://hxx.sjlbkw.cn

Go:   err.Error()
来源：http://ezj.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://azj.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://mtc.cheryme.top

[H09] 带错误码的异常
来源：http://vgj.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kwv.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dpb.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://axf.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vzq.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://onu.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zgn.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://hgu.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ytv.nanxuanxn.top

[H10] 资源自动释放
来源：http://xzq.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://whw.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dsd.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xks.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iuo.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fbk.yongpay.top

Go:   defer f.Close()
来源：http://iwl.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rvt.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cae.zdqjudy.top

================================================================================
来源：http://cnz.nanxinkj.top

I. 正则表达式
来源：http://gtj.ctjpmb.com

================================================================================
来源：http://yib.sweek.top

[I01] 判断是否匹配
来源：http://bgb.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eyf.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://puy.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://ama.fehbvm.com

TS:   /\d+/.test(s)
来源：http://kie.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://skq.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jlu.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://zyo.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ctb.aibaodan.cn

[I02] 提取所有匹配
来源：http://trm.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://fje.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xcx.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ups.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://lkf.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mdh.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nfz.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://wwe.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oai.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://ivk.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gfj.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jqr.zhoulong.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qit.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lqx.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wew.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rvc.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://znk.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://usk.nanxuanxn.top

[I04] 正则替换
来源：http://zsb.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://arn.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fwi.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://gjd.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://uxp.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://iou.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zfs.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ssp.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xjm.daria6918.cn

[I05] 按正则拆分
来源：http://edz.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://emh.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jjd.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://djz.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://gev.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://wyo.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ahe.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://jqx.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://itv.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://voc.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jag.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mkl.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vvn.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yvr.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qdh.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tyh.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ksz.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://owh.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://dfv.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jnq.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ixs.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lnm.shzxlz.cn

TS:   /error/gim
来源：http://tqb.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oxg.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mvp.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://hkm.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ezx.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://vfd.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hte.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ius.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mcz.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ihb.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://emf.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fyr.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yrv.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dog.cucudq.cn

================================================================================
来源：http://mxi.yfazqb.com

J. 日期与时间
来源：http://iuq.zdqjudy.top

================================================================================
来源：http://kob.sjlbkw.cn

[J01] 获取当前时间
来源：http://zoy.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yji.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sea.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://lsw.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://bim.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ean.sxryk.cn

Go:   time.Now()
来源：http://oak.hcnkem.com

Ruby: Time.now
来源：http://jks.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tcv.hnqzz.top

[J02] 格式化输出
来源：http://cld.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dyi.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kvl.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mlu.nanxuanxn.top

TS:   d.toISOString()
来源：http://qvu.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hxe.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ugp.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jte.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oii.sysykeji.top

[J03] 字符串解析为日期
来源：http://pbj.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ojq.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nle.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://uti.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://umm.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://wsw.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xqc.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://aca.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fdl.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://unr.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vth.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eni.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wlf.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dno.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qww.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gps.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cbt.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ugw.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://cri.uphjek.com

Py:   now + timedelta(days=7)
来源：http://iof.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ulx.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nch.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://guk.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://itu.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mzb.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://cks.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://emx.wangdashe.top

[J06] 计算两时间之差
来源：http://kvl.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://myj.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://ple.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dbt.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nlj.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://mqd.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://opk.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://hjn.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://xnk.andypj.xyz

[J07] 比较两个日期
来源：http://ztm.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://oop.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ewe.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ygq.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://azw.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xgp.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cnt.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ddy.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://sku.dashuyun.cn

[J08] 提取年月日与星期
来源：http://omj.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://adn.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cxa.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bbh.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nig.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tfl.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nbm.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rbr.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dvg.zycfv.cn

[J09] 时区处理
来源：http://eet.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zum.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rbs.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cii.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gqr.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bbi.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://viu.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bqd.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://waw.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://wyr.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rks.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ths.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dqm.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lzz.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mhz.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nof.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wvg.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jyt.yj202588.top

================================================================================
来源：http://pme.tianlin.xyz

K. JSON 与序列化
来源：http://mev.tanke756.top

================================================================================
来源：http://dnr.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://oga.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://myp.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jcg.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://ciw.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://shl.yj202588.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kli.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://sou.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://gpy.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uzt.xylfe.cn

[K02] JSON 字符串转对象
来源：http://nwa.chenlongwang.top

Py:   json.loads(s)
来源：http://vmd.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eqm.redwolf501.top

JS:   JSON.parse(s)
来源：http://hti.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://diz.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sxt.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://vzl.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://fpt.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bnf.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://adg.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tsk.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fbn.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ikf.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vxt.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ppn.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qlk.zhongyouzk.top


<!-- 参考信息 -->