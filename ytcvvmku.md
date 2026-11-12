代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://bmq.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://axp.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://ukt.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vks.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://zke.smart0.xyz

JS:   Object.entries(obj)
来源：http://zwi.hammf.cn

TS:   Object.entries(obj)
来源：http://qfg.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kgf.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://awk.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://hae.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://vxq.ehwqpu.com

================================================================================
来源：http://tvi.jqgfzy.top

H. 异常与错误处理
来源：http://sxr.havefunace.top

================================================================================
来源：http://hkm.yj20258.top

[H01] try / catch 基础
来源：http://krz.hnxiangtu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vcq.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pzn.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ext.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cqf.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bbs.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wrz.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gwf.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tsn.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://aig.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://fje.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://npc.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vmh.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tmc.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://xle.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://iir.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lte.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cqf.xuanzx.com

[H03] 主动抛出异常
来源：http://xzo.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://rqw.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kla.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://yjt.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://hns.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xqo.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bwp.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://eab.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://lde.c1oappe.top

[H04] 自定义异常类型
来源：http://ijq.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://oai.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://iye.cheryme.top

JS:   class MyError extends Error {}
来源：http://kkv.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://xfg.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://tnp.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ynf.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://jlf.cheryme.top

C#:   class MyException : Exception {}
来源：http://czd.sysykeji.top

[H05] 捕获特定类型
来源：http://vgn.bbcook.cn

Py:   except ValueError as e:
来源：http://fkj.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cmh.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://fmq.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://dwb.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://wzh.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eye.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://skx.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://syf.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://bim.fengsongda.top

Py:   value = d.get("k") or default
来源：http://cfm.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://jib.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://cih.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://usb.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dng.hammf.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yds.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://crf.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://khz.zhijiandao.cn

[H07] 断言
来源：http://dqj.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://iyi.vehdjk.com

PHP:  assert($x > 0);
来源：http://rto.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://moy.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://sqa.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://lhk.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lyd.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://flp.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://qbh.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://gmd.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://uvv.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://myg.ehwqpu.com

JS:   e.message;  e.stack
来源：http://kek.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qil.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hyg.cqqwz.cn

Go:   err.Error()
来源：http://zwy.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://kzd.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://ygf.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://cux.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://enz.aizwys.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ows.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fgn.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://upr.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nrz.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uck.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ezs.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mvk.zhongyouzk.top

[H10] 资源自动释放
来源：http://sfs.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://wpd.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jdg.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pvt.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pim.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oya.ppjwa.cn

Go:   defer f.Close()
来源：http://vcv.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qim.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nxk.sxryk.cn

================================================================================
来源：http://wkf.gzhubu.top

I. 正则表达式
来源：http://bai.ivvv.top

================================================================================
来源：http://bzj.kuanghao11.cn

[I01] 判断是否匹配
来源：http://mkl.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ncu.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sfp.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://fif.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://pde.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wgb.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rwd.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://gwq.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kti.aizwys.cn

[I02] 提取所有匹配
来源：http://taj.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://iws.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vgp.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lvm.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://nkx.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yxr.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fas.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://rho.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uxd.mhx1999.top

[I03] 提取捕获分组
来源：http://hev.ivvv.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nwi.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://otq.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ixv.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cwq.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ogu.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://smf.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rov.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dby.ppjwa.cn

[I04] 正则替换
来源：http://aqd.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://unt.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://quh.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://bjj.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://vnr.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://erf.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://pzs.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gyf.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://odg.zhiwuduotai.top

[I05] 按正则拆分
来源：http://ped.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cmt.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xjz.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://ddg.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://obe.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://ydw.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wht.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mmc.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xcj.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uzn.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awb.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xan.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cyi.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hgj.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://str.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gwd.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://piz.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gel.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://uhb.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blt.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cum.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vbm.guannengcc.top

TS:   /error/gim
来源：http://sdn.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cjo.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gyd.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://gff.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://efm.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://byu.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iyo.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ebj.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zhf.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pim.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ekh.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gls.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hxp.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xgx.redwolf501.top

================================================================================
来源：http://kwe.ydjk.org.cn

J. 日期与时间
来源：http://dci.jinghuilouyu.cn

================================================================================
来源：http://jbn.fktsv.cn

[J01] 获取当前时间
来源：http://edh.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://brv.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nbl.fzhhl.top

JS:   new Date();  Date.now()
来源：http://kis.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://btk.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qob.xziqi.cn

Go:   time.Now()
来源：http://aer.ppjwa.cn

Ruby: Time.now
来源：http://elp.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fak.hammf.cn

[J02] 格式化输出
来源：http://ncv.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ypf.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iwe.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lkx.shangyingyoupin.top

TS:   d.toISOString()
来源：http://lrj.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dfn.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://twh.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rbx.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://krs.chenzaomai.com

[J03] 字符串解析为日期
来源：http://hgb.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gqm.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bin.cashguo.top

JS:   new Date("2024-01-02")
来源：http://ary.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://icw.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://trv.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://exu.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://gzn.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oqk.guannengcc.top

[J04] 时间戳与日期互转
来源：http://gkd.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uqg.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zfd.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aik.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://urj.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ycs.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dew.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cqv.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://efv.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://uyf.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://jqa.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://waj.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cpv.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pqo.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://nwd.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hgz.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://kjg.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://taz.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://tjv.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://bzs.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://skt.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hvi.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mqf.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://kfz.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://mnc.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://maz.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://pkz.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://fxg.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://bfn.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://skh.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://ihl.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://qgu.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gky.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tbf.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://apm.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://blh.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://mbz.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vlf.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vwt.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uqa.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qym.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://heo.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://njp.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xtx.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kjg.zhijiandao.cn

[J09] 时区处理
来源：http://nzu.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://chf.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dvp.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xyp.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ctb.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ciu.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cbg.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qxo.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tfq.sweek.top

[J10] 取今天 / 本月第一天
来源：http://akf.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bmk.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://udt.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://enw.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bcr.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qwj.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tde.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://saq.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fbn.hesvh.cn

================================================================================
来源：http://ocb.yvedp.cn

K. JSON 与序列化
来源：http://own.meibo888.top

================================================================================
来源：http://xct.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://tmw.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rbx.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zgu.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://zpf.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://oiz.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pdu.hesvh.cn

Go:   json.Marshal(obj)
来源：http://jrp.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gkf.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://srv.tanke756.top

[K02] JSON 字符串转对象
来源：http://fqb.epnwcf.com

Py:   json.loads(s)
来源：http://ezg.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fwi.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://ion.dashuyun.cn

TS:   JSON.parse(s)
来源：http://yqw.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kay.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://zyw.hnqzz.top

Ruby: JSON.parse(s)
来源：http://lsm.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bfq.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://aql.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://enu.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vej.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ord.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iui.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qbr.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zbk.ctjpmb.com


<!-- 参考信息 -->