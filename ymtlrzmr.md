代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://foa.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tjl.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://khk.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mok.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://pdi.fengsongda.top

JS:   Object.entries(obj)
来源：http://ika.hammf.cn

TS:   Object.entries(obj)
来源：http://qik.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hhm.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hws.nanxinkj.top

Ruby: obj.instance_variables
来源：http://tkx.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://jhu.sysykeji.top

================================================================================
来源：http://eib.shangyingyoupin.top

H. 异常与错误处理
来源：http://srt.mhx1999.top

================================================================================
来源：http://dpo.chenlongwang.top

[H01] try / catch 基础
来源：http://yvp.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ddh.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uex.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xil.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://puz.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://imu.aizwys.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pqv.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cki.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gqp.daria6918.cn

[H02] finally / ensure 收尾
来源：http://jfy.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uez.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gwo.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://azj.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://own.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://vas.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mgn.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ucc.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://urz.52xcode.cn

[H03] 主动抛出异常
来源：http://zke.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://mah.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uue.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://pzu.hammf.cn

TS:   throw new Error("错误信息");
来源：http://qct.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dfb.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qjp.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://coj.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://wwm.guowangkeji.top

[H04] 自定义异常类型
来源：http://eou.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://del.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://enj.sxryk.cn

JS:   class MyError extends Error {}
来源：http://wpg.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://oxk.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://euo.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://unp.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://bmq.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://exv.zhoulong.xyz

[H05] 捕获特定类型
来源：http://ynf.uphjek.com

Py:   except ValueError as e:
来源：http://gjb.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://acl.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://qgv.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://pex.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://nko.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jky.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://yri.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ldg.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://dvo.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://zxm.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://ewr.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://llu.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://qcd.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dxn.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jjx.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://tfw.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://gwp.epnwcf.com

[H07] 断言
来源：http://tnv.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://mss.yueranfly.top

PHP:  assert($x > 0);
来源：http://aud.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://zar.hesvh.cn

TS:   console.assert(x > 0);
来源：http://iqj.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://fuv.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xct.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://scn.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://jhb.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://hyg.fktsv.cn

Py:   str(e);  traceback.format_exc()
来源：http://ttm.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lir.jianghu66.top

JS:   e.message;  e.stack
来源：http://yqt.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://utg.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mbd.shanyushiyangtech.top

Go:   err.Error()
来源：http://amn.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://zgp.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://tom.jinqigufen.top

[H09] 带错误码的异常
来源：http://fvv.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rdw.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://heq.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dun.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hts.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lre.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wmu.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kno.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bvc.uphjek.com

[H10] 资源自动释放
来源：http://oqb.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lbm.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tax.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dpy.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nae.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ndz.dashuyun.cn

Go:   defer f.Close()
来源：http://mid.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gwo.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://njy.xinyue.icu

================================================================================
来源：http://kis.zhoulong.xyz

I. 正则表达式
来源：http://dau.xingfuxueyuan.xyz

================================================================================
来源：http://sca.smart0.xyz

[I01] 判断是否匹配
来源：http://rpe.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fff.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://zjy.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://lyq.bjfxy.top

TS:   /\d+/.test(s)
来源：http://bgs.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://adi.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsh.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://vqx.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iss.nanxinkj.top

[I02] 提取所有匹配
来源：http://svp.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://zif.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://skr.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jdx.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://rcg.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lnw.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gbn.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://ebf.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kpf.jinqigufen.top

[I03] 提取捕获分组
来源：http://ynt.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pua.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pou.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rdw.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ntj.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jji.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://afd.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://roc.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hzq.sjlbkw.cn

[I04] 正则替换
来源：http://cpn.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xsf.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jlc.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lfm.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://zbn.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eum.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ysc.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nfl.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dci.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://nsi.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wzo.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://inn.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://soa.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://xvo.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://wkf.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://taw.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://xod.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lgr.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ebs.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bld.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zsn.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfn.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tpi.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ljz.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xeq.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cyw.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iye.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://qit.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bwk.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sfw.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rhl.hnqzz.top

TS:   /error/gim
来源：http://ohu.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tpr.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://afy.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://xfu.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uio.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://gxv.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iqa.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cma.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aws.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpk.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ljb.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qoh.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tsa.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lfu.hcnkem.com

================================================================================
来源：http://tzi.wangdashe.top

J. 日期与时间
来源：http://xbz.zhongyouzk.top

================================================================================
来源：http://yve.yuxming.cn

[J01] 获取当前时间
来源：http://pjw.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oeu.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dtn.sufxvd.cn

JS:   new Date();  Date.now()
来源：http://bds.sxryk.cn

TS:   new Date();  Date.now()
来源：http://lls.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gcf.mhx1999.top

Go:   time.Now()
来源：http://kru.xziqi.cn

Ruby: Time.now
来源：http://jya.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rcp.jqgufenzy.top

[J02] 格式化输出
来源：http://eou.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qpk.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ymu.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iny.hfpthk.cn

TS:   d.toISOString()
来源：http://doa.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://syg.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uob.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yvp.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oru.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://jrv.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rwf.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ulq.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://waa.havefunace.top

TS:   new Date("2024-01-02")
来源：http://irc.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hpz.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tbt.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://irh.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mko.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://ipw.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://acy.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gdo.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wke.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jyd.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lpz.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nin.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mup.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gjp.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://vgv.meibo888.top

Py:   now + timedelta(days=7)
来源：http://hpj.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jeg.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tok.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eja.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://koe.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xpj.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://jvy.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://vyl.vqdsnc.cn

[J06] 计算两时间之差
来源：http://mhp.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://zao.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://ely.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rse.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://izy.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://qbu.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://irn.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://gaf.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://vkj.birdmap.top

[J07] 比较两个日期
来源：http://kjs.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://gdm.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ddr.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://mho.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tfk.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://omt.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://egz.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://tza.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://hct.havefunace.top

[J08] 提取年月日与星期
来源：http://hkm.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://taz.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ztw.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ppx.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rji.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dvm.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aup.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zpx.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://llb.hysaishi.cn

[J09] 时区处理
来源：http://mvd.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hjx.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vmy.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bvf.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ecw.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mbp.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mld.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://xna.ydjk.org.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tjf.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://rtn.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zid.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cuc.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ili.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nfj.feifeiyinyue.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://huy.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vsa.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ppo.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zwv.jinqigfzy.top

================================================================================
来源：http://cct.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://ywk.wangshuangyany.cn

================================================================================
来源：http://yul.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://dqf.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://typ.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hwk.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://zid.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://jej.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bar.tarul.cn

Go:   json.Marshal(obj)
来源：http://bpn.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://xsz.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gyh.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://ibi.fzhhl.top

Py:   json.loads(s)
来源：http://xvr.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jjg.zhixingplan.top

JS:   JSON.parse(s)
来源：http://wvj.sweek.top

TS:   JSON.parse(s)
来源：http://erv.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fav.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://wyn.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://rxk.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bmo.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://gwq.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nqh.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tzb.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mga.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hjq.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tay.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://thf.ivvv.top


<!-- 参考信息 -->