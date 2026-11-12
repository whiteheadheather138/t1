代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ewk.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cxp.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://vas.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fsb.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://hoc.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xts.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://rgm.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://slw.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://zga.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://zjm.epnwcf.com

TS:   Object.entries(obj)
来源：http://zhd.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vsc.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://ohe.gogol.net.cn

Ruby: obj.instance_variables
来源：http://osk.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://sjo.xuanzx.com

================================================================================
来源：http://lag.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://hvx.sysykeji.top

================================================================================
来源：http://xwb.cashguo.top

[H01] try / catch 基础
来源：http://dsv.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kdj.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nbj.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xbl.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qrc.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nmz.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ghs.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zfq.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mqy.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://nqo.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://tjq.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lxg.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://eqb.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gew.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dfj.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xot.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cez.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ets.dashuyun.cn

[H03] 主动抛出异常
来源：http://prl.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://smp.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rwz.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://ccy.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://rqy.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jss.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lto.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hyl.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://qwe.bjfxy.top

[H04] 自定义异常类型
来源：http://kin.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://fyt.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://lta.jiagoushi.top

JS:   class MyError extends Error {}
来源：http://nas.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://mlt.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://bjx.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xjp.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://mrn.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://kkf.fktsv.cn

[H05] 捕获特定类型
来源：http://hfb.meibo888.top

Py:   except ValueError as e:
来源：http://ekq.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aqv.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://xgh.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://pdt.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://uyu.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hug.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://qay.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://osd.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://nrh.jianghu66.top

Py:   value = d.get("k") or default
来源：http://fzq.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://wjt.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://noq.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://kow.52xcode.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://osj.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jrs.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://tmb.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://vln.fehbvm.com

[H07] 断言
来源：http://lbx.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://aat.aizwys.cn

PHP:  assert($x > 0);
来源：http://oon.tarul.cn

JS:   console.assert(x > 0);
来源：http://zhg.daria6918.cn

TS:   console.assert(x > 0);
来源：http://ebh.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://mtr.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xnj.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://nwh.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://qyc.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://jtq.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://zks.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tyq.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://jzs.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ato.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oph.xuanzx.com

Go:   err.Error()
来源：http://lfn.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://uoc.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://xpe.nwbrower.top

[H09] 带错误码的异常
来源：http://dwd.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://plj.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kej.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jlo.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://evq.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rip.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hky.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://ibd.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qdt.cucudq.cn

[H10] 资源自动释放
来源：http://vdd.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://umh.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eae.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xjv.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://boj.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fly.cashguo.top

Go:   defer f.Close()
来源：http://eoa.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fjs.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xas.yuxming.cn

================================================================================
来源：http://fzj.pengpengdd.cyou

I. 正则表达式
来源：http://vqc.shanyushiyangtech.top

================================================================================
来源：http://bzu.yj20258.top

[I01] 判断是否匹配
来源：http://uwa.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tuk.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dkp.sxryk.cn

JS:   /\d+/.test(s)
来源：http://dwu.sysykeji.top

TS:   /\d+/.test(s)
来源：http://nbu.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qdu.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kpe.havefunace.top

Ruby: s.match?(/\d+/)
来源：http://mcj.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zzg.dianchejie.cn

[I02] 提取所有匹配
来源：http://fct.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://ngg.yonumen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tpa.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cdo.yonumen.top

TS:   s.match(/\d+/g)
来源：http://aqy.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wpq.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://egz.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://lik.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jvt.aizwys.cn

[I03] 提取捕获分组
来源：http://abo.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cvz.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://txy.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://icu.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tgc.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tex.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nrz.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://evb.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ylu.cucudq.cn

[I04] 正则替换
来源：http://pwu.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pww.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ukd.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gto.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://zzl.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://jqn.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zig.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xpn.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jbt.jyoumei.cn

[I05] 按正则拆分
来源：http://gzg.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ugi.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ivt.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://gsp.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://qtj.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://oir.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lso.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://exc.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://chk.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xih.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ins.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bux.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ikq.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqe.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dir.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gzs.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nml.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nqu.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://xzk.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ogn.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vqp.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vnt.jinghuilouyu.cn

TS:   /error/gim
来源：http://zke.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fru.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://flh.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://fvz.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ujv.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://pht.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wfp.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://unn.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xho.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qog.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sjw.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bpu.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://see.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yjv.xingfuxueyuan.xyz

================================================================================
来源：http://pct.xingfuxueyuan.xyz

J. 日期与时间
来源：http://ylf.hammf.cn

================================================================================
来源：http://jfo.ppjwa.cn

[J01] 获取当前时间
来源：http://vah.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jrq.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hbs.bbcook.cn

JS:   new Date();  Date.now()
来源：http://gvl.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://wsy.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dix.yuxming.cn

Go:   time.Now()
来源：http://mgn.hfpthk.cn

Ruby: Time.now
来源：http://wit.chenlongwang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rqn.yanxiufei.cn

[J02] 格式化输出
来源：http://ycg.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mzm.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kri.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nio.yangfankeji.com

TS:   d.toISOString()
来源：http://kns.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dej.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qlg.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jnw.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iis.aibaodan.cn

[J03] 字符串解析为日期
来源：http://tnr.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bat.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zhw.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://wao.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://guf.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://nhk.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://miw.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://sqv.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sst.xuanzx.com

[J04] 时间戳与日期互转
来源：http://bxl.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ght.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eli.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://awy.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dby.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eao.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mfe.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://brh.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hug.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://bhf.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://kjh.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://brv.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://upf.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://phs.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://qyv.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qna.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://rkt.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://srx.yvedp.cn

[J06] 计算两时间之差
来源：http://rsp.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://hur.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://nkt.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://suy.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ont.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://lbl.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://fcv.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://ali.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://qer.yonumen.top

[J07] 比较两个日期
来源：http://efc.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://pun.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kyf.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://her.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hcw.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ydn.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ioe.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://clp.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://ovo.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://jiv.cheryme.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pjm.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fze.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zsc.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xkn.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dgr.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zfh.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tqj.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pfh.sufxvd.cn

[J09] 时区处理
来源：http://ype.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lua.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nmz.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fia.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://far.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sph.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ick.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dcp.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xat.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://rqk.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://pxh.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gpe.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://atx.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://adi.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zsi.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ifb.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hlo.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://epj.mhx1999.top

================================================================================
来源：http://ala.guannengcc.top

K. JSON 与序列化
来源：http://ncq.jianghu66.top

================================================================================
来源：http://exw.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://kfv.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rhv.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://agp.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://stn.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://eol.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://izr.yj20258.top

Go:   json.Marshal(obj)
来源：http://ibv.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://yry.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qpo.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://jqv.daria6918.cn

Py:   json.loads(s)
来源：http://byf.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zue.sysykeji.top

JS:   JSON.parse(s)
来源：http://sot.tanke756.top

TS:   JSON.parse(s)
来源：http://pcl.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gyq.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://ipl.iojbl.cn

Ruby: JSON.parse(s)
来源：http://usw.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://csk.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://kfw.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fqk.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xjg.cucudq.cn


<!-- 参考信息 -->