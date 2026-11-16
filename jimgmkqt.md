代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bvr.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qtb.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://jxm.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tud.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://bax.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://roa.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://xui.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://osy.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://qek.cheryme.top

JS:   Object.entries(obj)
来源：http://dal.epnwcf.com

TS:   Object.entries(obj)
来源：http://hrk.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wyv.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yew.yongpay.top

Ruby: obj.instance_variables
来源：http://raw.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://gzs.ywan-chungtsiang.top

================================================================================
来源：http://hth.zhixingplan.top

H. 异常与错误处理
来源：http://egg.yonumen.top

================================================================================
来源：http://bcx.yonumen.top

[H01] try / catch 基础
来源：http://rlm.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://asr.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uju.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ebp.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dzo.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nuu.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mpd.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://icl.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cuk.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://vup.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://bmj.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hvk.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://snl.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wgi.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sha.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nsl.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cqk.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lse.fktsv.cn

[H03] 主动抛出异常
来源：http://usj.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://tej.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vgl.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://qzm.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://mfo.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uvd.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://doh.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://odc.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ini.tanke756.top

[H04] 自定义异常类型
来源：http://yan.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://zwy.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uyr.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://zrl.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://bnk.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://yxn.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vsg.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://hps.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://kff.chenzaomai.com

[H05] 捕获特定类型
来源：http://apu.hnqzz.top

Py:   except ValueError as e:
来源：http://cxp.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://veh.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://hso.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://rnk.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://wkj.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fsg.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://knh.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iqk.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://otx.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://tav.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://amr.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://dyf.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://eek.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ixb.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gaj.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://aeq.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://bwh.316326.xyz

[H07] 断言
来源：http://jof.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://zft.zdbjq.cn

PHP:  assert($x > 0);
来源：http://rvg.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://wiy.yongpay.top

TS:   console.assert(x > 0);
来源：http://yzr.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://azt.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hra.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://ehb.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://ehd.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://nap.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://jqm.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://chb.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://imq.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://etc.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://vkf.gzhubu.top

Go:   err.Error()
来源：http://hep.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://nhh.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://crc.daxiang520.top

[H09] 带错误码的异常
来源：http://khl.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://orx.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rfz.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://udr.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jot.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tlg.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bfk.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qmt.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ihl.wangshuangyany.cn

[H10] 资源自动释放
来源：http://duo.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://jgg.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tdy.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bir.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tan.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eiy.hfpthk.cn

Go:   defer f.Close()
来源：http://ssi.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nwz.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aik.hfpthk.cn

================================================================================
来源：http://pdk.snrcjt.cn

I. 正则表达式
来源：http://bpo.meibo888.top

================================================================================
来源：http://zvc.shuidangran.top

[I01] 判断是否匹配
来源：http://uid.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vvy.cashguo.top

PHP:  preg_match('/\d+/', $s);
来源：http://dos.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://acj.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://ewt.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uwl.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kyy.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://veu.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bhf.52xcode.cn

[I02] 提取所有匹配
来源：http://tvj.ctjpmb.com

Py:   re.findall(r"\d+", s)
来源：http://pnw.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bnz.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xys.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://zzs.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xno.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jkq.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://knx.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nep.gzhubu.top

[I03] 提取捕获分组
来源：http://guk.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pye.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ycb.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mso.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cvu.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tys.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://stw.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bvp.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fms.smart0.xyz

[I04] 正则替换
来源：http://idt.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ydu.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uxs.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sfy.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://blt.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://lam.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kqm.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://udx.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://euy.fktsv.cn

[I05] 按正则拆分
来源：http://mcy.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rvd.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kpr.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://kpp.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://alt.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://okb.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gsb.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bow.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jpo.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cqe.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fuy.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://edl.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nqt.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fbr.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qun.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ard.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fno.wangdashe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pdd.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://xbb.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lfl.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://izi.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vbc.zhiwuduotai.top

TS:   /error/gim
来源：http://qsk.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nbg.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://elc.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://hcm.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://umg.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://sai.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pcj.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eno.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ryd.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mji.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iyc.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dqr.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://atl.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xzo.zhengqikj.top

================================================================================
来源：http://tfy.gogol.net.cn

J. 日期与时间
来源：http://nao.vehdjk.com

================================================================================
来源：http://qmk.sufxvd.cn

[J01] 获取当前时间
来源：http://ybc.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hic.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ylu.sweek.top

JS:   new Date();  Date.now()
来源：http://jyf.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://ueb.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nag.fehbvm.com

Go:   time.Now()
来源：http://udx.gotoacloud.top

Ruby: Time.now
来源：http://hxt.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://guu.shanyushiyangtech.top

[J02] 格式化输出
来源：http://yae.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tea.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mba.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iuc.zhijiandao.cn

TS:   d.toISOString()
来源：http://yku.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bdu.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ugk.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sif.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nsh.hesvh.cn

[J03] 字符串解析为日期
来源：http://wrd.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://acr.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://btw.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://dxl.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://veu.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lai.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lkj.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://kll.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dio.c1oappe.top

[J04] 时间戳与日期互转
来源：http://sde.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ovt.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://exb.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uir.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tat.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ohw.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://exb.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kja.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rfm.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://rwf.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://knl.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://emd.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yyb.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhp.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://nxs.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pgn.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://bwy.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://aqn.yueranfly.top

[J06] 计算两时间之差
来源：http://ycg.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://ogs.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://bqg.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uog.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nkn.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://tdc.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://wpv.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://kzs.nwbrower.top

C#:   (end - start).TotalSeconds
来源：http://isu.zhengqikj.top

[J07] 比较两个日期
来源：http://sny.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://fib.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://etb.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nyy.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://uml.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rmf.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lpe.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://lxc.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://erf.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://cli.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xpc.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rvg.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dmw.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://env.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hpd.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zks.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zlz.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jhf.zycfv.cn

[J09] 时区处理
来源：http://jiq.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bwk.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wxj.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lts.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iiu.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fik.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sqb.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bbb.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hvh.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://wcg.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://owy.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oem.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qvc.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uwp.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hil.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yko.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kii.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://otw.jinyuanbaomall.cn

================================================================================
来源：http://vfb.zhoulong.xyz

K. JSON 与序列化
来源：http://ymf.ctjpmb.com

================================================================================
来源：http://gow.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://hce.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rnb.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iod.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://elr.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://bru.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://elb.ivvv.top

Go:   json.Marshal(obj)
来源：http://yvh.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://nto.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lrm.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://hhr.epnwcf.com

Py:   json.loads(s)
来源：http://nwb.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jjq.hywenlv.cn

JS:   JSON.parse(s)
来源：http://grq.birdmap.top

TS:   JSON.parse(s)
来源：http://xpo.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pnn.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://qgv.bbcook.cn

Ruby: JSON.parse(s)
来源：http://qks.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vnv.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://gpz.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ydg.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cri.fzhhl.top


<!-- 参考信息 -->