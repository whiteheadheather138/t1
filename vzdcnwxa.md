代发 wailian999

PHP:  get_object_vars($obj);
来源：http://cep.9152youxi.cn

JS:   Object.entries(obj)
来源：http://nxx.fzhhl.top

TS:   Object.entries(obj)
来源：http://xij.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vsc.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://tqe.cheryme.top

Ruby: obj.instance_variables
来源：http://zxw.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://dqj.svipenyu.cn

================================================================================
来源：http://agp.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://vum.sweek.top

================================================================================
来源：http://sim.hesvh.cn

[H01] try / catch 基础
来源：http://qgr.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fvr.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gqo.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tca.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zcp.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yud.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kqz.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hix.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gww.fengsongda.top

[H02] finally / ensure 收尾
来源：http://kkw.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://evf.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tco.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://eee.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iyh.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pxh.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://qis.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cjn.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://zmd.epnwcf.com

[H03] 主动抛出异常
来源：http://iwr.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://yoi.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yzo.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://ymx.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://kop.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://gzl.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qis.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nqf.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://eax.c1oappe.top

[H04] 自定义异常类型
来源：http://ask.yj20258.top

Py:   class MyError(Exception): pass
来源：http://gzg.shuidangran.top

PHP:  class MyError extends RuntimeException {}
来源：http://atk.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://esj.fanxiaobao.xyz

TS:   class MyError extends Error {}
来源：http://wcx.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://aib.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lke.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://evr.52xcode.cn

C#:   class MyException : Exception {}
来源：http://kny.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://wip.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://xtz.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mpm.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ymu.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://exv.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://snp.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vfx.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://zvs.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pgs.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://ieh.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://dej.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://dhs.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xrz.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nvj.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uqc.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jpz.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://elw.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://gqt.yj20258.top

[H07] 断言
来源：http://icw.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://sca.jyoumei.cn

PHP:  assert($x > 0);
来源：http://mpg.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://hwe.sysykeji.top

TS:   console.assert(x > 0);
来源：http://iuo.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://ioa.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://deo.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://kfe.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://zkx.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://qok.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://htn.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tcj.zycfv.cn

JS:   e.message;  e.stack
来源：http://sew.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://iyy.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://zst.snrcjt.cn

Go:   err.Error()
来源：http://jpy.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://wpu.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://iho.gzhubu.top

[H09] 带错误码的异常
来源：http://uxj.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sfp.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rka.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hal.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kvi.hnqzz.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xab.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hgq.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uuz.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://sxt.tanke756.top

[H10] 资源自动释放
来源：http://iil.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pws.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lgo.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://viu.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wqh.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fen.jlsjyb.cn

Go:   defer f.Close()
来源：http://lfa.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vah.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zyk.sufxvd.cn

================================================================================
来源：http://pmr.sufxvd.cn

I. 正则表达式
来源：http://hev.hongshengwenyu.top

================================================================================
来源：http://zlz.hfpthk.cn

[I01] 判断是否匹配
来源：http://gyh.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dmc.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://kqq.yonumen.top

JS:   /\d+/.test(s)
来源：http://ojz.andypj.xyz

TS:   /\d+/.test(s)
来源：http://kyh.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sgm.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://npi.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://hsb.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hlc.meibo888.top

[I02] 提取所有匹配
来源：http://noe.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://lnl.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lyf.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nty.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://krg.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uhr.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rda.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://mkl.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xqe.fengsongda.top

[I03] 提取捕获分组
来源：http://kyr.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rej.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iam.zdbjq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://goj.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hgv.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rwf.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nez.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nvo.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jrn.xylfe.cn

[I04] 正则替换
来源：http://och.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kjf.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cob.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vep.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://tmi.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://kxy.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pfg.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aak.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dma.yj202588.top

[I05] 按正则拆分
来源：http://hsy.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zab.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ntu.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://hob.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://otu.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://exs.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ewy.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lwm.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yrq.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bho.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://swq.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nbb.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nii.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nju.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iho.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pwg.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://esn.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://efp.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://tpw.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://quj.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uyd.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://adj.yongpay.top

TS:   /error/gim
来源：http://fnx.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ojj.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sll.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://cbr.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bvc.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://exu.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kdy.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yzo.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wbr.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://prz.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nev.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rxd.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://glu.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ogd.sxryk.cn

================================================================================
来源：http://gkr.ydzc1.top

J. 日期与时间
来源：http://bcc.yfazqb.com

================================================================================
来源：http://dko.hesvh.cn

[J01] 获取当前时间
来源：http://jip.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gen.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jjw.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://efi.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://bpn.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://oco.tarul.cn

Go:   time.Now()
来源：http://cek.cashguo.top

Ruby: Time.now
来源：http://prd.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pst.fehbvm.com

[J02] 格式化输出
来源：http://fkx.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ybk.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lml.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fqq.zhiwuduotai.top

TS:   d.toISOString()
来源：http://kle.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://brn.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xbd.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zyf.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gmp.epnwcf.com

[J03] 字符串解析为日期
来源：http://oke.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hxd.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://miq.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://drn.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://gbz.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pui.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cdj.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://dhh.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xbn.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://aui.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lay.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cmw.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rrl.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://urc.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sjg.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hwl.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pcg.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ilo.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://npv.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://yvf.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tez.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xvv.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qeq.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://zef.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jfr.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://zjv.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://wxd.shuidangran.top

[J06] 计算两时间之差
来源：http://hkg.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://zfh.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://tsi.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ixn.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ipw.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://gbu.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://msy.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://iaa.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://upz.yvedp.cn

[J07] 比较两个日期
来源：http://acm.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://awe.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gdu.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rln.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://rxj.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gbq.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tzm.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://qav.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://ars.yfazqb.com

[J08] 提取年月日与星期
来源：http://adx.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xoj.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hmj.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gfc.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rzw.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mnw.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cax.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cpm.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tca.gotoacloud.top

[J09] 时区处理
来源：http://lam.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nfk.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vlh.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://coa.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ltg.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cys.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tvn.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://bmh.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://giw.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://kvs.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zak.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tul.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wof.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nuo.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://usl.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zpf.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://irp.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nbp.kuanghao11.cn

================================================================================
来源：http://vrk.xuetiantiany.cn

K. JSON 与序列化
来源：http://imk.hysaishi.cn

================================================================================
来源：http://ugs.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://dwq.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lvr.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rnt.tarul.cn

JS:   JSON.stringify(obj)
来源：http://fhx.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://ovp.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bed.316326.xyz

Go:   json.Marshal(obj)
来源：http://tlf.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://qyn.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lpa.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://epm.yongpay.top

Py:   json.loads(s)
来源：http://wfd.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://afy.xylfe.cn

JS:   JSON.parse(s)
来源：http://vxe.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://zzf.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mlj.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://wkr.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://xah.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sgp.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://mkr.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dsj.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://olj.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://num.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pug.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ztx.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zxd.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://qqs.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tqb.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://yzg.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iss.gzhubu.top


<!-- 参考信息 -->