代发 wailian999

C#:   record User(string Name, int Age);
来源：http://vxk.gzhubu.top

[G15] 枚举
来源：http://elg.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qvh.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pch.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wac.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qzt.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://rcc.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dcj.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://euu.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nwn.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://ubx.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://scv.havefunace.top

PHP:  get_object_vars($obj);
来源：http://lnf.ppjwa.cn

JS:   Object.entries(obj)
来源：http://woi.hfpthk.cn

TS:   Object.entries(obj)
来源：http://ped.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qfj.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://amg.yj202588.top

Ruby: obj.instance_variables
来源：http://vlb.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://pcp.yvedp.cn

================================================================================
来源：http://jnq.hysaishi.cn

H. 异常与错误处理
来源：http://uqa.meibo888.top

================================================================================
来源：http://trd.hysaishi.cn

[H01] try / catch 基础
来源：http://ich.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zyp.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kvf.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://svo.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qru.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://afb.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ovd.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gkf.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://glv.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://ozb.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iqm.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bet.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oaa.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jmz.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://zvc.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vdp.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ulg.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://pef.jqgufenzy.top

[H03] 主动抛出异常
来源：http://udh.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://mwj.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uip.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://wnv.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://xwt.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hdz.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yzo.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://qex.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://egv.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://hug.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://imc.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jgc.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://hhi.hesvh.cn

TS:   class MyError extends Error {}
来源：http://zng.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://qxi.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ekz.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://wbo.fktsv.cn

C#:   class MyException : Exception {}
来源：http://zzd.xuanzx.com

[H05] 捕获特定类型
来源：http://nzl.hfpthk.cn

Py:   except ValueError as e:
来源：http://kcs.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://umr.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://mso.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://ife.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://jas.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lfe.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://cwn.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rtc.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://pac.vehdjk.com

Py:   value = d.get("k") or default
来源：http://oet.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kjn.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://jca.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://dgz.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fwe.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ooo.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://lry.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://ygl.tanke756.top

[H07] 断言
来源：http://dnt.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://ikr.chenzaomai.com

PHP:  assert($x > 0);
来源：http://ddt.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://tqy.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://ova.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://jny.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cmc.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jqb.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://eaq.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://ycr.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://srr.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qvb.guowangkeji.top

JS:   e.message;  e.stack
来源：http://arp.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pym.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jkp.ydzc1.top

Go:   err.Error()
来源：http://awd.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://avo.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://iwb.havefunace.top

[H09] 带错误码的异常
来源：http://ztc.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rtt.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kgf.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jjc.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tuw.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aut.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://otl.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://vdl.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jta.fzhhl.top

[H10] 资源自动释放
来源：http://omp.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ssi.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ydk.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mma.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hnp.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vgn.chenjidiqi.icu

Go:   defer f.Close()
来源：http://lzj.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rgg.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nff.ppjwa.cn

================================================================================
来源：http://nhd.xingfuxueyuan.xyz

I. 正则表达式
来源：http://hkn.chenlongwang.top

================================================================================
来源：http://ugx.daxiang520.top

[I01] 判断是否匹配
来源：http://nyu.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gny.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://pvo.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://eds.birdmap.top

TS:   /\d+/.test(s)
来源：http://sal.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sez.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qyg.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://yip.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ajx.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://usb.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://wfh.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fsx.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ywl.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://rim.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bco.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tdf.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://qqv.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cbn.yfazqb.com

[I03] 提取捕获分组
来源：http://mqr.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wkm.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fog.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vsa.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ckf.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zyx.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ffs.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fjj.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aev.xylfe.cn

[I04] 正则替换
来源：http://iot.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ybc.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yos.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ccp.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://yxy.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://pya.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://blj.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zsn.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kgo.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://amj.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wdr.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bau.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://mhc.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://rpo.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://xid.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qsw.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://qlv.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yfj.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rbo.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lqa.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hqe.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyp.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jqt.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wpy.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pjs.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wre.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mmu.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://rfw.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lki.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rpy.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://die.snrcjt.cn

TS:   /error/gim
来源：http://zws.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kka.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zsu.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://rof.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rgi.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://qak.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lxz.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mkl.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cwg.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxe.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tdk.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gcl.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://veh.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xgi.shangyingyoupin.top

================================================================================
来源：http://ddw.smart0.xyz

J. 日期与时间
来源：http://dkd.hongshengwenyu.top

================================================================================
来源：http://len.aibaodan.cn

[J01] 获取当前时间
来源：http://mpw.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bxr.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dns.fehbvm.com

JS:   new Date();  Date.now()
来源：http://kbi.ydzc1.top

TS:   new Date();  Date.now()
来源：http://xqm.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ocf.jianghu66.top

Go:   time.Now()
来源：http://ouy.epnwcf.com

Ruby: Time.now
来源：http://gjy.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xpk.aibaodan.cn

[J02] 格式化输出
来源：http://phc.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rjm.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zfc.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tco.jqgufenzy.top

TS:   d.toISOString()
来源：http://rur.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hbs.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rev.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qxh.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uiw.yj202588.top

[J03] 字符串解析为日期
来源：http://lav.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vhq.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zhp.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://zmd.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://kxz.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://wjg.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bqu.9152youxi.cn

Ruby: Date.parse("2024-01-02")
来源：http://zyt.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cdp.aizwys.cn

[J04] 时间戳与日期互转
来源：http://jae.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vgf.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tol.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uas.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sny.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jwh.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gdx.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gfk.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jwn.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://sdw.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://bge.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://tyv.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hya.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ekn.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://pwn.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kce.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://kno.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lzg.shuidangran.top

[J06] 计算两时间之差
来源：http://tuu.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://ivj.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://qnc.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bac.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://acp.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iph.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://cdv.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://ugz.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://dqj.ppjwa.cn

[J07] 比较两个日期
来源：http://gki.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://elu.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ggs.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://wfy.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://nmh.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ire.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vfw.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lto.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://voh.yuanzhike.top

[J08] 提取年月日与星期
来源：http://gze.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xqt.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bvw.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cby.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lrg.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cpr.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qmd.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bpq.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://txs.tarul.cn

[J09] 时区处理
来源：http://nxw.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cmi.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qnk.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aba.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://plt.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wmm.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nkp.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://axm.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jtk.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://ltp.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iol.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fas.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uey.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lch.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vsr.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qgl.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tho.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jol.zhoulong.xyz

================================================================================
来源：http://mie.ybcxt.top

K. JSON 与序列化
来源：http://xzv.ctjpmb.com

================================================================================
来源：http://cfr.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://nvn.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hqi.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iba.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://loe.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://eow.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qrc.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://kxh.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cuo.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lis.hammf.cn

[K02] JSON 字符串转对象
来源：http://vdu.ehwqpu.com

Py:   json.loads(s)
来源：http://izr.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sds.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://xqi.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://djq.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pub.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://lco.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://oym.iojbl.cn


<!-- 参考信息 -->