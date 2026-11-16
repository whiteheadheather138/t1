代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://jrd.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://xre.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://ttw.hcnkem.com

================================================================================
来源：http://rsk.sufxvd.cn

H. 异常与错误处理
来源：http://zui.cdnleiting.top

================================================================================
来源：http://yvb.vqdsnc.cn

[H01] try / catch 基础
来源：http://zys.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pwz.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wue.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kpj.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ciu.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vlo.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vki.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pwd.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sls.daxiang520.top

[H02] finally / ensure 收尾
来源：http://hhc.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hwd.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vdj.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lyb.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cps.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://qdz.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qtu.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cgl.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zav.hnqzz.top

[H03] 主动抛出异常
来源：http://gyf.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://vfy.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://poc.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://ybh.ivvv.top

TS:   throw new Error("错误信息");
来源：http://dzv.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://hrs.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kmj.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rse.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uwq.zhijiandao.cn

[H04] 自定义异常类型
来源：http://zid.uphjek.com

Py:   class MyError(Exception): pass
来源：http://exg.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://nox.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://vfh.yvedp.cn

TS:   class MyError extends Error {}
来源：http://nrb.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://fzp.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wlc.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://wsh.sweek.top

C#:   class MyException : Exception {}
来源：http://tim.mhx1999.top

[H05] 捕获特定类型
来源：http://gar.yangfankeji.com

Py:   except ValueError as e:
来源：http://wye.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ido.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://cbq.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://kmp.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://qde.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cia.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://dbh.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wsq.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://cyq.fengsongda.top

Py:   value = d.get("k") or default
来源：http://dcy.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bnf.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oyx.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://hrk.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yju.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yxm.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://qrc.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://gzx.nwbrower.top

[H07] 断言
来源：http://odg.jinqigufen.top

Py:   assert x > 0, "必须为正"
来源：http://yjj.daxiang520.top

PHP:  assert($x > 0);
来源：http://gqn.316326.xyz

JS:   console.assert(x > 0);
来源：http://ohs.bbcook.cn

TS:   console.assert(x > 0);
来源：http://xgr.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://kcp.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://czs.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://zrp.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://mzd.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://tnj.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://zrk.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tym.yueranfly.top

JS:   e.message;  e.stack
来源：http://kak.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oup.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://fbd.zhijiandao.cn

Go:   err.Error()
来源：http://ydg.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://dop.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://sds.meibo888.top

[H09] 带错误码的异常
来源：http://pzy.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jeq.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tok.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eze.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://giz.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sbp.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rsu.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tfz.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://amb.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://vvu.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ipe.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nfh.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cad.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eto.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jve.havefunace.top

Go:   defer f.Close()
来源：http://hkl.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fxw.redwolf501.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iwj.redwolf501.top

================================================================================
来源：http://zjs.zhongyouzk.top

I. 正则表达式
来源：http://pzp.fktsv.cn

================================================================================
来源：http://xzi.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://wcj.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hjc.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://udf.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://cop.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://akp.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ari.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uum.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://esj.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cdv.snrcjt.cn

[I02] 提取所有匹配
来源：http://axk.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://uvk.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ron.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://otv.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://ijk.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ixp.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pgp.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://zbj.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yep.xuanzx.com

[I03] 提取捕获分组
来源：http://lga.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gxg.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hfh.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dxc.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ela.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kcc.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wqt.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iiw.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bqg.daria6918.cn

[I04] 正则替换
来源：http://gtl.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xcp.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rvg.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://ccs.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://mql.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://isq.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jqv.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xmm.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vrq.hnqzz.top

[I05] 按正则拆分
来源：http://knr.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eyn.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xbp.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://ijr.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://xmo.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://jjb.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fxt.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://wvh.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qft.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rij.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sog.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jyv.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eig.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baz.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kzg.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://syk.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sdu.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://evh.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://umk.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fxz.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dhw.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mey.fktsv.cn

TS:   /error/gim
来源：http://wvp.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hyy.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ect.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://the.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://enb.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://bad.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://utg.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yzz.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vcf.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxu.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://hny.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ohs.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vti.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gbp.ctjpmb.com

================================================================================
来源：http://jyh.yfazqb.com

J. 日期与时间
来源：http://sji.xingfuxueyuan.xyz

================================================================================
来源：http://ctg.zhijiandao.cn

[J01] 获取当前时间
来源：http://nay.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mjl.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lhb.c1oappe.top

JS:   new Date();  Date.now()
来源：http://qsi.fzhhl.top

TS:   new Date();  Date.now()
来源：http://bcz.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qtv.yongpay.top

Go:   time.Now()
来源：http://yat.epnwcf.com

Ruby: Time.now
来源：http://uzo.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dui.zhijiandao.cn

[J02] 格式化输出
来源：http://xxi.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jsa.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nvy.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hph.bjfxy.top

TS:   d.toISOString()
来源：http://xil.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zvu.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mon.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fth.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qgt.xinyue.icu

[J03] 字符串解析为日期
来源：http://ysg.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://msj.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qmm.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://gfr.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://wrm.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zlu.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://stw.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://hca.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://din.mhx1999.top

[J04] 时间戳与日期互转
来源：http://djz.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hbh.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://crk.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://upt.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hed.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kuz.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://znz.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jkt.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tlu.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://and.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://ofi.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ubm.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://khp.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uha.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://kgu.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://few.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://qeh.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://woc.bjfxy.top

[J06] 计算两时间之差
来源：http://auu.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://mcr.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://ykj.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fhs.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zmw.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mjb.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://aak.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://aad.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://ake.cheryme.top

[J07] 比较两个日期
来源：http://ozc.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://quv.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gyv.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://dho.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://fgx.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dfg.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bqu.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hpb.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://lmr.ivvv.top

[J08] 提取年月日与星期
来源：http://rkb.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mal.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uor.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yvz.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jbg.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ucr.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ijf.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xqu.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jmh.wangdashe.top

[J09] 时区处理
来源：http://bwb.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://svs.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://olb.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wty.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://stz.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jvs.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tqk.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sml.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zvw.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://hjl.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fcu.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lyz.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uia.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kam.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mfg.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iga.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://azl.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qrs.xylfe.cn

================================================================================
来源：http://ozw.pengpengdd.cyou

K. JSON 与序列化
来源：http://bzh.svipenyu.cn

================================================================================
来源：http://erk.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://myb.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vgm.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qlx.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://cxt.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://isv.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mqv.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://tql.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://oqt.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hcr.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://eox.ydjk.org.cn

Py:   json.loads(s)
来源：http://ysj.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ojk.52xcode.cn

JS:   JSON.parse(s)
来源：http://xpr.sufxvd.cn

TS:   JSON.parse(s)
来源：http://vmo.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cuy.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://zsn.sysykeji.top

Ruby: JSON.parse(s)
来源：http://nfo.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xrx.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://dlc.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://adu.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zvc.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jpp.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zsf.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wcs.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vdc.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://dnm.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ojx.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://fra.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sro.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vqx.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hib.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sgl.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hhe.shuidangran.top


<!-- 参考信息 -->