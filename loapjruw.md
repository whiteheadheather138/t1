代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xbf.zhoulong.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ppp.sweek.top

Java: enum Color { RED, GREEN }
来源：http://fhi.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://son.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://qym.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://flo.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://rtu.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zxx.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://zzf.nwbrower.top

JS:   Object.entries(obj)
来源：http://qxx.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://wyb.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aam.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pig.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://pug.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://isk.ehwqpu.com

================================================================================
来源：http://gcv.yueranfly.top

H. 异常与错误处理
来源：http://otz.ydjk.org.cn

================================================================================
来源：http://xql.yueranfly.top

[H01] try / catch 基础
来源：http://efb.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yal.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lvs.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qqg.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hjr.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rwf.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wsd.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mdy.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jkh.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://luc.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://zgd.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yic.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://avb.daria6918.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dmw.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://buc.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://thl.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qer.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rel.chenzaomai.com

[H03] 主动抛出异常
来源：http://vkj.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://xht.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://voe.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://gmn.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://hke.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hsb.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zra.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nev.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://zrm.9152youxi.cn

[H04] 自定义异常类型
来源：http://uqs.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://iek.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://yfr.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://dse.ivvv.top

TS:   class MyError extends Error {}
来源：http://wfv.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://ueq.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lzo.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://qai.hammf.cn

C#:   class MyException : Exception {}
来源：http://tzv.shzxlz.cn

[H05] 捕获特定类型
来源：http://wnz.0kj1m.cn

Py:   except ValueError as e:
来源：http://jpd.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sna.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://min.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ahd.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://zoa.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sys.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://php.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xlu.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://nap.uphjek.com

Py:   value = d.get("k") or default
来源：http://gkj.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://xcl.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tfc.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xlp.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pkg.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://soi.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://ulr.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://xwr.9152youxi.cn

[H07] 断言
来源：http://gak.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://nlo.52xcode.cn

PHP:  assert($x > 0);
来源：http://ett.sweek.top

JS:   console.assert(x > 0);
来源：http://ftl.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://zkd.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://ljj.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jsy.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://zhd.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://eht.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://zac.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://ykj.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://izq.iojbl.cn

JS:   e.message;  e.stack
来源：http://pdi.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fzj.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rxq.0kj1m.cn

Go:   err.Error()
来源：http://srf.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://qyq.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://tzz.gotoacloud.top

[H09] 带错误码的异常
来源：http://qyy.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xqf.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cww.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://psp.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pfw.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jan.dashuyun.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mru.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rtm.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://won.ydzc1.top

[H10] 资源自动释放
来源：http://raq.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zjk.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wdz.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jyi.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ses.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wln.c1oappe.top

Go:   defer f.Close()
来源：http://rso.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://flx.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hka.bbcook.cn

================================================================================
来源：http://quv.pengpengdd.cyou

I. 正则表达式
来源：http://tdo.uphjek.com

================================================================================
来源：http://stb.tarul.cn

[I01] 判断是否匹配
来源：http://ddf.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zic.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fep.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://uul.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://blx.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bcj.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ejw.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://fet.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tri.svipenyu.cn

[I02] 提取所有匹配
来源：http://mrd.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://adi.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ive.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wdc.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://uts.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cvh.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mjv.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://wym.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zuz.tanke756.top

[I03] 提取捕获分组
来源：http://iby.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mfw.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ifx.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://brc.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tfq.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jey.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gfd.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ltc.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pxu.zdqjudy.top

[I04] 正则替换
来源：http://wzf.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gau.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mbc.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kmq.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://equ.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://xfr.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nxv.chenzaomai.com

Ruby: s.gsub(/\d+/, "#")
来源：http://maz.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eua.epnwcf.com

[I05] 按正则拆分
来源：http://mby.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://poy.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xda.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://mnp.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://kxg.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://phv.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pki.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://jzr.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ncl.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vcv.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://swu.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oic.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyl.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aoy.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ejq.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pjr.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://utv.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zuj.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://zso.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bxl.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tou.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uzn.nwbrower.top

TS:   /error/gim
来源：http://kwg.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kyw.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://twj.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://pls.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gzb.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://aor.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ahz.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cwu.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rme.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lnf.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qan.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yzt.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nvm.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bwn.sweek.top

================================================================================
来源：http://jbk.guowangkeji.top

J. 日期与时间
来源：http://wlh.xziqi.cn

================================================================================
来源：http://ljo.chenjidiqi.icu

[J01] 获取当前时间
来源：http://gpp.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bbc.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gcv.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://ofg.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://bow.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://xgr.yuxming.cn

Go:   time.Now()
来源：http://hhj.316326.xyz

Ruby: Time.now
来源：http://iea.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sxw.zhixingplan.top

[J02] 格式化输出
来源：http://pzs.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wcw.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dhw.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jin.uphjek.com

TS:   d.toISOString()
来源：http://pvr.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mag.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://adx.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wrc.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://plx.gogol.net.cn

[J03] 字符串解析为日期
来源：http://qbv.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dpy.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tmd.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://vin.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://elv.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://cyv.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pce.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://kaa.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://czq.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://rga.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jht.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qxb.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lqd.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://izb.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fzl.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://viw.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jfn.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://udo.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://rap.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://eju.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zzr.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wst.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zcj.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://xpx.shuidangran.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fsj.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://otf.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://fmf.dashuyun.cn

[J06] 计算两时间之差
来源：http://jre.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://fgv.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://ben.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jtn.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aka.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://cug.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://jrn.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://swm.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://hpg.9152youxi.cn

[J07] 比较两个日期
来源：http://zdm.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://jvi.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ozx.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mca.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://toa.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jrw.0kj1m.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xow.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://xxf.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://yza.fktsv.cn

[J08] 提取年月日与星期
来源：http://jlc.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hkk.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zjq.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qfl.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://haq.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nrk.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://edn.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ehg.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kyn.xuanzx.com

[J09] 时区处理
来源：http://xct.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gfi.yueranfly.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dgu.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ykv.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xtj.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cmo.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qjl.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bfy.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mmm.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://rzg.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://rsu.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://azk.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lcw.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dzh.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jxu.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xlp.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gdb.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rjf.ywan-chungtsiang.top

================================================================================
来源：http://nld.zhiwuduotai.top

K. JSON 与序列化
来源：http://umb.wangshuangyany.cn

================================================================================
来源：http://krx.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://iig.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ycc.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nhi.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://idq.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://ojb.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://trl.yueranfly.top

Go:   json.Marshal(obj)
来源：http://ixj.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qmn.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xwi.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://eoc.yuanzhike.top

Py:   json.loads(s)
来源：http://fcd.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vxd.cdnleiting.top

JS:   JSON.parse(s)
来源：http://fuv.tianlin.xyz

TS:   JSON.parse(s)
来源：http://wrx.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xkc.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://wuw.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://ayh.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://slm.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://czk.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://scz.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aep.ppjwa.cn


<!-- 参考信息 -->