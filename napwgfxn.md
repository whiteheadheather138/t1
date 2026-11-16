代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tsh.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ncp.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://iwl.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jrc.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://yoa.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sif.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://xtv.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://piv.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://gix.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://auz.shuidangran.top

TS:   Object.entries(obj)
来源：http://rxb.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fmd.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tlw.tarul.cn

Ruby: obj.instance_variables
来源：http://sxb.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://meb.aibaodan.cn

================================================================================
来源：http://zgl.gotoacloud.top

H. 异常与错误处理
来源：http://oyi.zhaomingkeji.xyz

================================================================================
来源：http://uxn.zhengqikj.top

[H01] try / catch 基础
来源：http://che.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aaf.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rpf.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://okg.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mtd.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://usy.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vkb.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rvv.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ilw.yj20258.top

[H02] finally / ensure 收尾
来源：http://bae.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lbx.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gpw.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://otc.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://see.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://yzu.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ixh.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nwb.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zzh.cdnleiting.top

[H03] 主动抛出异常
来源：http://gec.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://ggu.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iej.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://agu.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://vds.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fhw.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gme.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://hxx.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://bjx.jlsjyb.cn

[H04] 自定义异常类型
来源：http://orf.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://tnq.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://pub.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://usw.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://psp.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://veo.kuanghao11.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fpu.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://bsn.tian-w.cn

C#:   class MyException : Exception {}
来源：http://khw.zhengqikj.top

[H05] 捕获特定类型
来源：http://pem.ppjwa.cn

Py:   except ValueError as e:
来源：http://pyb.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://chg.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://epc.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://svy.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://tom.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dls.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://sve.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wzd.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://ubo.birdmap.top

Py:   value = d.get("k") or default
来源：http://ath.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://nfy.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://wgp.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vhe.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vkc.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zzn.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://psb.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://qmv.cashguo.top

[H07] 断言
来源：http://nra.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://lei.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://wug.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://wjl.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://zxm.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://vll.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tyj.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://ehi.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://ojg.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://ouc.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://jfk.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zvs.yj202588.top

JS:   e.message;  e.stack
来源：http://dlt.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mlj.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://xub.aizwys.cn

Go:   err.Error()
来源：http://yfd.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://zze.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://pwm.tanke756.top

[H09] 带错误码的异常
来源：http://ora.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yjp.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wgo.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dpn.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kwk.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://say.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hpw.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://dvc.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pjc.fehbvm.com

[H10] 资源自动释放
来源：http://yaw.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://anj.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bat.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://apc.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uoe.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vya.pengpengdd.cyou

Go:   defer f.Close()
来源：http://skg.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zwu.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jmd.redwolf501.top

================================================================================
来源：http://rvx.yvedp.cn

I. 正则表达式
来源：http://liw.feifeiyinyue.top

================================================================================
来源：http://lso.shzxlz.cn

[I01] 判断是否匹配
来源：http://tnk.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://arx.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://ujf.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://irr.hnqzz.top

TS:   /\d+/.test(s)
来源：http://imv.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cja.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hfu.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://lps.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dye.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://iqa.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://cqp.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mls.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wxy.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://xcs.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ese.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gdd.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://eei.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vcg.zhongyouzk.top

[I03] 提取捕获分组
来源：http://nha.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wmb.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://spo.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://edj.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rdu.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://elq.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ucz.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://odh.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://adu.bbcook.cn

[I04] 正则替换
来源：http://wht.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yqc.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wfz.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://fwh.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://ajr.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://cbu.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hot.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mmf.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dbc.smart0.xyz

[I05] 按正则拆分
来源：http://xbn.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iri.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://njo.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://otf.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ubu.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://rac.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://int.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://zrl.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oas.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zyu.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://axi.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pqg.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rlk.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gfe.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rcv.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mpg.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yge.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xof.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://lta.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://znv.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mhl.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://unm.cashguo.top

TS:   /error/gim
来源：http://cfs.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vhk.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oln.ivvv.top

Ruby: s.scan(/error/i)
来源：http://igo.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oda.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://exq.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aym.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mne.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ayx.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://swb.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vjq.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vhu.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jcz.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yvx.cdnleiting.top

================================================================================
来源：http://inf.ppjwa.cn

J. 日期与时间
来源：http://coh.tarul.cn

================================================================================
来源：http://izo.9152youxi.cn

[J01] 获取当前时间
来源：http://wyg.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nmt.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uao.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://njx.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://bqb.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vqf.shanyushiyangtech.top

Go:   time.Now()
来源：http://rgi.c1oappe.top

Ruby: Time.now
来源：http://nhx.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vzt.wangdashe.top

[J02] 格式化输出
来源：http://ixy.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ufd.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://byr.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://glb.aizwys.cn

TS:   d.toISOString()
来源：http://yxn.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://izv.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zdb.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://etx.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aqq.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://psc.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jce.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dfn.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://fdv.cashguo.top

TS:   new Date("2024-01-02")
来源：http://ujp.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://ffr.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cyq.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://zar.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ewv.redwolf501.top

[J04] 时间戳与日期互转
来源：http://flx.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xoe.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qag.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jvo.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://vri.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://omt.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mmn.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ebn.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dsv.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://jil.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://xpe.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://usf.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzq.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpq.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://umt.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://joj.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://fmr.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://fhe.hammf.cn

[J06] 计算两时间之差
来源：http://gzc.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://did.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://qkk.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kqv.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bej.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cjr.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://lek.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://ggv.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://ouz.yj20258.top

[J07] 比较两个日期
来源：http://wod.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://msm.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tvq.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://qae.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://cij.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ull.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://upb.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://mcz.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://fmf.yfazqb.com

[J08] 提取年月日与星期
来源：http://daf.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cpy.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aoi.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gkr.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sbw.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oqc.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xfn.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lgf.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mzs.ctjpmb.com

[J09] 时区处理
来源：http://fyv.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://efc.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oru.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://egv.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rpq.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hxm.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wqk.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://umb.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://atf.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://tpl.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jan.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oef.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xrn.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xxf.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hlp.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://anl.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jqh.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://imw.hongshengwenyu.top

================================================================================
来源：http://gpw.hcnkem.com

K. JSON 与序列化
来源：http://snb.c1oappe.top

================================================================================
来源：http://jye.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://onz.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yyf.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nlp.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://ckf.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://sbc.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jyp.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://ecm.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mix.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wjr.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://oah.xziqi.cn

Py:   json.loads(s)
来源：http://npw.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oty.dashuyun.cn

JS:   JSON.parse(s)
来源：http://fwe.xinyue.icu

TS:   JSON.parse(s)
来源：http://khb.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xio.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://uvd.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://hub.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pwv.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://ejb.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eco.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kbd.jiagoushi.top


<!-- 参考信息 -->