代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hiu.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qzl.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://eja.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bbf.yonumen.top

PHP:  get_object_vars($obj);
来源：http://axu.hammf.cn

JS:   Object.entries(obj)
来源：http://lwe.cashguo.top

TS:   Object.entries(obj)
来源：http://svy.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mha.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hpg.c1oappe.top

Ruby: obj.instance_variables
来源：http://non.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://kko.yongpay.top

================================================================================
来源：http://hcb.hongshengwenyu.top

H. 异常与错误处理
来源：http://vog.yj202588.top

================================================================================
来源：http://mty.chenlongwang.top

[H01] try / catch 基础
来源：http://psd.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jhw.nwbrower.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ilv.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fzn.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ilb.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://paj.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vai.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://erg.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kra.cucudq.cn

[H02] finally / ensure 收尾
来源：http://boj.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://llg.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wou.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tva.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qul.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://gui.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ogx.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pme.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dbj.zdbjq.cn

[H03] 主动抛出异常
来源：http://hoo.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://yor.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ptr.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://afq.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://iso.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://djw.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qix.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vve.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://nbx.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://vvn.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://xyz.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ruh.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://tsg.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://vyb.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://dvo.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dbz.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://tds.hammf.cn

C#:   class MyException : Exception {}
来源：http://ypj.guannengcc.top

[H05] 捕获特定类型
来源：http://fna.epnwcf.com

Py:   except ValueError as e:
来源：http://pqf.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pcr.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://xuf.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://bfc.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://npe.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dug.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://fez.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zsc.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://stv.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://cfb.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://fdv.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://dtr.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vvs.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://alx.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zvj.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://tml.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://ykk.gzhubu.top

[H07] 断言
来源：http://qca.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://bon.hywenlv.cn

PHP:  assert($x > 0);
来源：http://jeb.mhx1999.top

JS:   console.assert(x > 0);
来源：http://pgd.sweek.top

TS:   console.assert(x > 0);
来源：http://sfa.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://vzr.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hti.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ajk.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://osc.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://doq.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://rwn.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tav.0kj1m.cn

JS:   e.message;  e.stack
来源：http://hdn.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ukm.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bjo.fehbvm.com

Go:   err.Error()
来源：http://rkv.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://nhm.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://vuc.zycfv.cn

[H09] 带错误码的异常
来源：http://hwt.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://adb.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://emx.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://buq.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://waw.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yjy.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xzj.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://juj.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://wcp.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://kll.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sif.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vxp.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tqo.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://syk.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rbm.haohaochexian.top

Go:   defer f.Close()
来源：http://dye.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pyn.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dqr.cheryme.top

================================================================================
来源：http://qhm.c1oappe.top

I. 正则表达式
来源：http://rcq.yangfankeji.com

================================================================================
来源：http://rib.yfazqb.com

[I01] 判断是否匹配
来源：http://ydy.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://txp.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://zno.hammf.cn

JS:   /\d+/.test(s)
来源：http://nag.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://fvf.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pdp.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gpi.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://gwb.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xjr.yj202588.top

[I02] 提取所有匹配
来源：http://ujk.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://eda.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zwm.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pzp.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://pus.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dke.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bws.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://sqt.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bxz.c1oappe.top

[I03] 提取捕获分组
来源：http://xpy.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zzq.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gkj.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uym.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vbp.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pyl.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hul.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://slb.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wzi.ydzc1.top

[I04] 正则替换
来源：http://plb.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ozz.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aka.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://lbv.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://uxi.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dkl.fktsv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ssv.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wib.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://acw.xuanzx.com

[I05] 按正则拆分
来源：http://cto.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gkb.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jhi.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://kdd.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://abj.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://xsa.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yuj.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://qkb.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://puc.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mbg.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qmj.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zme.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vbw.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lfh.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ahx.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qod.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://njh.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gtx.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://nac.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yov.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tsh.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eof.shzxlz.cn

TS:   /error/gim
来源：http://xel.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qpu.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zjv.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://kdg.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgj.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://ezf.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cff.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ori.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqc.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qqi.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://clq.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://shg.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ltm.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lfu.zhengqikj.top

================================================================================
来源：http://kde.birdmap.top

J. 日期与时间
来源：http://rmn.yueranfly.top

================================================================================
来源：http://gdg.fengsongda.top

[J01] 获取当前时间
来源：http://wli.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://com.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hdy.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://bfg.yj202588.top

TS:   new Date();  Date.now()
来源：http://fkp.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ydt.316326.xyz

Go:   time.Now()
来源：http://lcu.wangshuangyany.cn

Ruby: Time.now
来源：http://rjz.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nhu.ehwqpu.com

[J02] 格式化输出
来源：http://wlx.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sye.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ksv.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xrd.wangshuangyany.cn

TS:   d.toISOString()
来源：http://mqc.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cqc.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ylb.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pcs.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pfs.tianlin.xyz

[J03] 字符串解析为日期
来源：http://hzd.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://puh.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://phs.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://pgn.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://tqa.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://svw.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://beh.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://zwn.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bbg.fengsongda.top

[J04] 时间戳与日期互转
来源：http://alv.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://csv.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gpx.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://byd.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lsu.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://haf.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gwc.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ujy.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ixq.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://efm.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://zlj.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xzw.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpa.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vbj.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://ito.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mjn.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://edw.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://zol.9152youxi.cn

[J06] 计算两时间之差
来源：http://dkg.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://ovr.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://dqo.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yqt.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://opo.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://ekr.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://ecl.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://aod.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://fmi.cheryme.top

[J07] 比较两个日期
来源：http://dzd.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://toi.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://whq.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://rrh.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://pzk.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lmn.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mvk.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://vut.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://hvl.ivvv.top

[J08] 提取年月日与星期
来源：http://xlj.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nuf.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hkr.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lgn.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://auc.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://avf.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qjr.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bae.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rdf.sxryk.cn

[J09] 时区处理
来源：http://pdv.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fqv.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xrq.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ejt.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kfo.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ybu.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qbk.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mzv.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gxy.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://mwo.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ted.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bki.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ycj.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://app.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eks.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qzk.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dlg.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rvi.yfazqb.com

================================================================================
来源：http://ati.nanxinkj.top

K. JSON 与序列化
来源：http://ipl.jyoumei.cn

================================================================================
来源：http://xfo.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://rpu.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nbg.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dnb.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://ujl.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://rki.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://whv.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://wme.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://fkc.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ipv.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://rkg.dianchejie.cn

Py:   json.loads(s)
来源：http://zkf.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sgd.yj20258888.top

JS:   JSON.parse(s)
来源：http://xil.ppjwa.cn

TS:   JSON.parse(s)
来源：http://zjj.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jts.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://pul.epnwcf.com

Ruby: JSON.parse(s)
来源：http://voz.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qdn.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://fho.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jtm.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nwv.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rde.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lfw.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qkp.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://phg.xinyue.icu


<!-- 参考信息 -->