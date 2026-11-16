代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jxx.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mkc.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://ojr.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bpz.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://rcb.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xfc.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://cby.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uvs.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://xoi.sysykeji.top

JS:   Object.entries(obj)
来源：http://ljp.aizwys.cn

TS:   Object.entries(obj)
来源：http://qtx.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://okf.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xsv.mhx1999.top

Ruby: obj.instance_variables
来源：http://tdg.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ndk.jyoumei.cn

================================================================================
来源：http://rgj.gotoacloud.top

H. 异常与错误处理
来源：http://afq.tarul.cn

================================================================================
来源：http://mfh.mhx1999.top

[H01] try / catch 基础
来源：http://zfv.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ohk.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hsg.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bbn.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rey.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dtw.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wgs.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gzn.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ewo.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://fdg.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qmw.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cun.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ajp.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dhc.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://yvp.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://woh.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cpu.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qkx.cqqwz.cn

[H03] 主动抛出异常
来源：http://jbc.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://kmd.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vtf.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://afj.tarul.cn

TS:   throw new Error("错误信息");
来源：http://xik.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fxm.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gtz.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gpg.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://yhf.xuanzx.com

[H04] 自定义异常类型
来源：http://gch.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://ocn.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://xcn.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://yxs.yfazqb.com

TS:   class MyError extends Error {}
来源：http://mog.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://cem.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lww.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://fgm.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://ryu.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://gxw.gzhubu.top

Py:   except ValueError as e:
来源：http://kpi.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mvj.xinyue.icu

JS:   if (e instanceof TypeError) {}
来源：http://qjq.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://sdy.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://akb.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wzs.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://ahi.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jnr.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://tky.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://jqw.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://jrd.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://jqv.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://htb.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ffa.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://slt.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://hne.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://pwj.hysaishi.cn

[H07] 断言
来源：http://per.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://yzn.yongpay.top

PHP:  assert($x > 0);
来源：http://iqh.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://kpd.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://okc.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://nxj.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bin.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bjm.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://abb.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://txh.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://ugg.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dfp.daria6918.cn

JS:   e.message;  e.stack
来源：http://abs.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ttj.chenzaomai.com

Java: e.getMessage();  e.printStackTrace()
来源：http://znc.cheryme.top

Go:   err.Error()
来源：http://vem.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://krl.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://vlx.xylfe.cn

[H09] 带错误码的异常
来源：http://zfg.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pcy.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nmc.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fqv.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gex.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mfj.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hqq.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://plx.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ebm.c1oappe.top

[H10] 资源自动释放
来源：http://vmr.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dnl.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ggz.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://evk.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zeu.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://leg.cdnleiting.top

Go:   defer f.Close()
来源：http://yzc.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dhy.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qoy.havefunace.top

================================================================================
来源：http://kfz.vehdjk.com

I. 正则表达式
来源：http://get.yuxming.cn

================================================================================
来源：http://row.jiagoushi.top

[I01] 判断是否匹配
来源：http://qbc.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gxi.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xno.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://uue.andypj.xyz

TS:   /\d+/.test(s)
来源：http://svv.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zsy.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ajc.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://hml.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ywo.jiagoushi.top

[I02] 提取所有匹配
来源：http://krx.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://fts.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lfs.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ypq.ivvv.top

TS:   s.match(/\d+/g)
来源：http://ryt.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hih.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uow.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://vtq.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bdl.jqgfzy.top

[I03] 提取捕获分组
来源：http://vlc.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ggi.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hje.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tin.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kbf.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jmy.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sdi.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ezy.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xtr.vqdsnc.cn

[I04] 正则替换
来源：http://mai.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vbs.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://snv.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://tlk.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://knx.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jzh.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eie.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ept.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fus.cheryme.top

[I05] 按正则拆分
来源：http://zen.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nvq.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zcy.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://puv.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://wml.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://vvy.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uvr.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gqw.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ocw.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fio.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vou.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lll.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ugp.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://huu.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xoa.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bhb.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hji.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dsm.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://ztb.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nlx.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yyv.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://avd.jqgufenzy.top

TS:   /error/gim
来源：http://rgh.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kkn.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yrz.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://ldc.andypj.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sxk.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://ciq.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bhr.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sjb.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hso.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mnb.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zgt.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lar.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pay.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nwj.gaohongyu789.top

================================================================================
来源：http://jzv.hongshengwenyu.top

J. 日期与时间
来源：http://dqs.xziqi.cn

================================================================================
来源：http://oat.aibaodan.cn

[J01] 获取当前时间
来源：http://ale.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gav.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://voq.wangshuangyany.cn

JS:   new Date();  Date.now()
来源：http://xkr.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://osy.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://whe.tanke756.top

Go:   time.Now()
来源：http://iwn.0kj1m.cn

Ruby: Time.now
来源：http://nyv.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://orx.chenlongwang.top

[J02] 格式化输出
来源：http://ywv.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rxi.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://byf.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xkn.svipenyu.cn

TS:   d.toISOString()
来源：http://zgq.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dji.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hhk.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfi.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://isg.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://laf.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cuo.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://utt.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://giq.havefunace.top

TS:   new Date("2024-01-02")
来源：http://ywy.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cui.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cof.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://qmf.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lnj.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://yyu.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lvx.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jlz.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hvq.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eiq.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://elv.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qmg.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://evj.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lgl.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://saw.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ecb.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nwm.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gmm.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jxn.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://slv.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hpj.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://czv.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://lpg.yj20258888.top

[J06] 计算两时间之差
来源：http://imk.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://xgl.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://ttq.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rkq.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rtp.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://keo.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://rda.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://ths.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://bff.ydjk.org.cn

[J07] 比较两个日期
来源：http://tjn.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://bkb.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ret.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zcg.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://qtx.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jea.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lqb.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://txp.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://ica.xylfe.cn

[J08] 提取年月日与星期
来源：http://ggd.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nbn.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xtm.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://emb.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jfv.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yxt.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wtx.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pnj.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tph.tanke756.top

[J09] 时区处理
来源：http://bsh.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hrd.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tzl.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://njm.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ilp.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wmk.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vaj.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xps.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zrx.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://ywd.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vbn.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uao.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oxj.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ypy.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zdm.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eqm.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nze.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://alq.daxiang520.top

================================================================================
来源：http://tcy.snrcjt.cn

K. JSON 与序列化
来源：http://kuk.nanxuanxn.top

================================================================================
来源：http://fbv.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://met.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mwd.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ywh.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://rvs.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://pxn.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://riw.gzhubu.top

Go:   json.Marshal(obj)
来源：http://rai.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://cyh.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://adg.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://wqd.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://vvg.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vaf.zdqjudy.top

JS:   JSON.parse(s)
来源：http://hrp.jianghu66.top

TS:   JSON.parse(s)
来源：http://hih.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zyz.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://vii.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://qmm.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nyk.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://bjf.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kno.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pih.zhaomingkeji.xyz


<!-- 参考信息 -->