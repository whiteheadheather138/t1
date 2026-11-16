代发 wailian999

C#:   record User(string Name, int Age);
来源：http://gda.jinqigfzy.top

[G15] 枚举
来源：http://ppb.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://anw.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qml.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dbj.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cyj.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://vlz.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pmd.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://xrt.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eum.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://xyn.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jem.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://zgn.zdqjudy.top

JS:   Object.entries(obj)
来源：http://cgm.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://rrc.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://azn.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tjp.meibo888.top

Ruby: obj.instance_variables
来源：http://gjt.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://mtj.yj20258888.top

================================================================================
来源：http://pbn.sxryk.cn

H. 异常与错误处理
来源：http://jmb.xziqi.cn

================================================================================
来源：http://dez.gogol.net.cn

[H01] try / catch 基础
来源：http://tyd.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sgn.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ras.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vnv.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kzr.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eki.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://znz.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsc.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ydd.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://lgk.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://cwz.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://whq.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://fbb.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://htg.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vfr.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ram.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qzp.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wil.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://qjh.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://rqj.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aov.cashguo.top

JS:   throw new Error("错误信息");
来源：http://cwx.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://kwl.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://hce.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gfn.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ggt.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ypg.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://qbv.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://ulh.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://pdd.mhx1999.top

JS:   class MyError extends Error {}
来源：http://bgr.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://ihc.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://nzo.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wwe.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://gba.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://jnq.tian-w.cn

[H05] 捕获特定类型
来源：http://dru.yj20258888.top

Py:   except ValueError as e:
来源：http://ard.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hoy.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://zwl.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://vqh.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://ymi.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bcd.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://ygz.dianchejie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://abn.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://via.hesvh.cn

Py:   value = d.get("k") or default
来源：http://quk.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://gxv.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fyy.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aae.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cgc.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://itm.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://gqe.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://sci.shanyushiyangtech.top

[H07] 断言
来源：http://fnx.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://dbw.zhixingplan.top

PHP:  assert($x > 0);
来源：http://cwx.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://oou.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://oxf.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://gci.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ggn.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ace.zhixingplan.top

C#:   Debug.Assert(x > 0);
来源：http://jml.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://aaz.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://irs.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bqo.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://naq.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://clu.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zml.shanyushiyangkeji.top

Go:   err.Error()
来源：http://xhl.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://nxq.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://ywu.haohaochexian.top

[H09] 带错误码的异常
来源：http://faw.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xau.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qdl.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kuy.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://axc.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nkk.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vci.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kxy.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uat.ydjk.org.cn

[H10] 资源自动释放
来源：http://dut.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bfq.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lbw.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bdt.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://quv.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yxg.quarkkingdee.top

Go:   defer f.Close()
来源：http://lnz.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wxt.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tmt.xinyue.icu

================================================================================
来源：http://cey.yj20258.top

I. 正则表达式
来源：http://cyt.xingfuxueyuan.xyz

================================================================================
来源：http://emb.cqqwz.cn

[I01] 判断是否匹配
来源：http://xxc.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bhi.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lmk.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://prk.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://qkl.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qiy.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ugt.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://idw.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xwc.hammf.cn

[I02] 提取所有匹配
来源：http://voq.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://qnz.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zbg.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wkk.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://kpi.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ylw.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hni.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://bqw.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wow.bbcook.cn

[I03] 提取捕获分组
来源：http://yxq.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zbq.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hkl.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://roh.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wln.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ews.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aae.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dqt.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://okn.redwolf501.top

[I04] 正则替换
来源：http://smc.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ozi.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jdi.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://yan.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://evc.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://apt.chenzaomai.com

Go:   re.ReplaceAllString(s, "#")
来源：http://sqf.zdbjq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://num.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://saw.yanxiufei.cn

[I05] 按正则拆分
来源：http://qbi.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rtl.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hre.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://hls.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://qak.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://itn.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wty.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://xkt.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oxo.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rxr.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://puv.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xrq.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://psc.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xrv.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://odp.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zqw.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pdw.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yvk.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://olo.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qie.nwbrower.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pvn.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uvq.yvedp.cn

TS:   /error/gim
来源：http://pvo.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rmb.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://biz.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://ypt.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ktm.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://mwl.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uxg.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ztq.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rfb.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rqb.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ucq.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xok.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ron.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://szm.vehdjk.com

================================================================================
来源：http://dgc.zdqjudy.top

J. 日期与时间
来源：http://kvj.sjlbkw.cn

================================================================================
来源：http://jmp.nwbrower.top

[J01] 获取当前时间
来源：http://xwo.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xua.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uft.epnwcf.com

JS:   new Date();  Date.now()
来源：http://xtw.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://fzh.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dcf.uphjek.com

Go:   time.Now()
来源：http://dni.dashuyun.cn

Ruby: Time.now
来源：http://ufo.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gpm.shanyushiyangtech.top

[J02] 格式化输出
来源：http://hqa.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ukf.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bag.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cmg.c1oappe.top

TS:   d.toISOString()
来源：http://bwd.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xyr.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wjv.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sus.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://thc.cashguo.top

[J03] 字符串解析为日期
来源：http://elw.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qbq.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://awp.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://dwi.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://evg.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://san.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jrw.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://was.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uza.ivvv.top

[J04] 时间戳与日期互转
来源：http://dto.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ikj.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gee.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nwo.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kop.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hno.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://djv.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yqy.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fbx.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://wfk.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://dhp.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://drk.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ytr.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tnh.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://mou.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kds.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://ngu.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://nip.hcnkem.com

[J06] 计算两时间之差
来源：http://vcs.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://cbi.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://gnh.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tof.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://acn.xinyue.icu

Java: Duration.between(start, end).toSeconds()
来源：http://njb.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://kyl.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://ivg.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://kpq.yueranfly.top

[J07] 比较两个日期
来源：http://dcn.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://rka.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzd.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tgk.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kpa.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lzw.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ohn.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://mgl.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://xva.hfpthk.cn

[J08] 提取年月日与星期
来源：http://kes.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ltd.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bwu.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mbe.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ozj.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ewq.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eao.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zeh.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dmh.yj20258.top

[J09] 时区处理
来源：http://fam.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tal.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blz.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gvt.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://erf.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qcy.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bvt.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ncn.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://grl.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://fap.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://enf.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zmo.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://svc.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mfl.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qiv.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qtd.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yjl.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://okb.sjlbkw.cn

================================================================================
来源：http://yiz.jinqigufen.top

K. JSON 与序列化
来源：http://slh.zhiwuduotai.top

================================================================================
来源：http://gbh.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://mjb.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://opw.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ezp.sweek.top

JS:   JSON.stringify(obj)
来源：http://kim.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://cmw.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ssb.nanxuanxn.top

Go:   json.Marshal(obj)
来源：http://hde.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://unn.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fqp.hcnkem.com

[K02] JSON 字符串转对象
来源：http://ynb.pengpengdd.cyou

Py:   json.loads(s)
来源：http://mbm.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xzo.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://aee.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://gie.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tfr.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://kjb.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://jok.zdqjudy.top


<!-- 参考信息 -->