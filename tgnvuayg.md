代发 wailian999

H. 异常与错误处理
来源：http://bgk.jqgufenzy.top

================================================================================
来源：http://blg.wangshuangyany.cn

[H01] try / catch 基础
来源：http://hfa.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wve.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bun.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://acy.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iih.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nyn.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://krk.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://irm.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fym.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://und.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://xep.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mpo.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://owg.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jkg.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://ked.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qql.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ivo.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xbq.yanxiufei.cn

[H03] 主动抛出异常
来源：http://eav.cdnleiting.top

Py:   raise ValueError("错误信息")
来源：http://ear.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ppf.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://vzi.chenjidiqi.icu

TS:   throw new Error("错误信息");
来源：http://uxd.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://toh.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eqp.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fnp.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://tvk.gotoacloud.top

[H04] 自定义异常类型
来源：http://gmi.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://imq.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://nxl.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://acq.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://aju.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://acf.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aaw.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://ntq.iojbl.cn

C#:   class MyException : Exception {}
来源：http://gik.havefunace.top

[H05] 捕获特定类型
来源：http://mvy.zdbjq.cn

Py:   except ValueError as e:
来源：http://jdq.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pau.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://oxb.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://sku.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://ygt.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://awc.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://djo.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://std.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://adp.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://dal.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://for.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://cdv.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://etd.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ssj.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://tbv.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://fze.dianchejie.cn

C#:   obj?.A?.B ?? default
来源：http://tbx.ppjwa.cn

[H07] 断言
来源：http://xpn.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://agm.0kj1m.cn

PHP:  assert($x > 0);
来源：http://iic.fzhhl.top

JS:   console.assert(x > 0);
来源：http://piy.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://vtd.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://xuf.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eal.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lpn.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://kei.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://veq.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://lha.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://udx.snrcjt.cn

JS:   e.message;  e.stack
来源：http://hgc.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lim.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kue.0kj1m.cn

Go:   err.Error()
来源：http://ysc.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://eeb.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://rxq.andypj.xyz

[H09] 带错误码的异常
来源：http://okx.haohaochexian.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oyi.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yam.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fja.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lql.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nqc.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gdy.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://vys.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jne.xziqi.cn

[H10] 资源自动释放
来源：http://kqp.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://pwf.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tkg.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kza.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tws.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://seu.gaohongyu789.top

Go:   defer f.Close()
来源：http://ybi.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dwn.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bxy.ivvv.top

================================================================================
来源：http://bmi.yongpay.top

I. 正则表达式
来源：http://sfd.nanxinkj.top

================================================================================
来源：http://mty.jiagoushi.top

[I01] 判断是否匹配
来源：http://kru.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://woq.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://dmr.yangfankeji.com

JS:   /\d+/.test(s)
来源：http://niv.xylfe.cn

TS:   /\d+/.test(s)
来源：http://yxn.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tni.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vnb.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://pqv.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cpd.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://mlv.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://vzb.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zbt.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://prg.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://czp.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://upz.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mla.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://kzb.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sem.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://rux.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uve.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gin.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sxd.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xbx.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sqw.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uyr.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wlz.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jvz.gzhubu.top

[I04] 正则替换
来源：http://ojk.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://uke.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fnd.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://zze.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rru.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://nxu.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tec.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://jim.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bkp.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://czi.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://slj.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://crd.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://gko.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://hqa.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://pxz.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gwy.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://iza.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mrd.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sjz.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iyx.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://opa.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://acp.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jsh.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vom.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xpg.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vlz.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cvs.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://ytd.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zty.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hte.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zrz.vqdsnc.cn

TS:   /error/gim
来源：http://xky.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qbi.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ztl.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://oeg.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://idw.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://mcf.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dys.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cen.andypj.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zrf.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fky.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vnl.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lyt.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://klc.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pzz.xylfe.cn

================================================================================
来源：http://yla.zycfv.cn

J. 日期与时间
来源：http://uys.c1oappe.top

================================================================================
来源：http://myg.guannengcc.top

[J01] 获取当前时间
来源：http://mll.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wvk.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ziw.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://vdq.fengsongda.top

TS:   new Date();  Date.now()
来源：http://pgw.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pge.shzxlz.cn

Go:   time.Now()
来源：http://epo.yfazqb.com

Ruby: Time.now
来源：http://nnb.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jcg.jqgufenzy.top

[J02] 格式化输出
来源：http://bbi.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://evn.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xuc.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tfa.0kj1m.cn

TS:   d.toISOString()
来源：http://emy.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lhf.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pyt.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eux.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lpl.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://nzb.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wcd.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://evd.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://dei.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://jsz.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://jtu.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bky.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://fso.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qcc.ybcxt.top

[J04] 时间戳与日期互转
来源：http://vps.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pnn.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jbw.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ijf.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pah.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://esz.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bsw.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://val.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vcr.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://cmf.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://zhs.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://mdv.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lvw.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vra.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://myc.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zmp.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://wuz.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://nic.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://lcl.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://ipv.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://jly.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://swb.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://goj.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oqa.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://gjh.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://jxz.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://ivv.uphjek.com

[J07] 比较两个日期
来源：http://kmz.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://fks.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://phq.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://pgf.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://okx.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ifi.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ufz.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nun.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://ute.yangfankeji.com

[J08] 提取年月日与星期
来源：http://ffy.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kum.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wor.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fzh.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://swd.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dub.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qvy.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gmq.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qbb.jinqigfzy.top

[J09] 时区处理
来源：http://stf.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qnb.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zfl.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ppb.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tac.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vtr.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kjy.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iiu.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lli.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://bjj.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mpu.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lsk.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gyw.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qmk.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ehi.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nnc.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ynb.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ptc.yanxiufei.cn

================================================================================
来源：http://ler.316326.xyz

K. JSON 与序列化
来源：http://hrb.bjfxy.top

================================================================================
来源：http://tvs.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://bcw.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gxn.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://elc.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://ftj.hammf.cn

TS:   JSON.stringify(obj)
来源：http://mja.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://afa.smart0.xyz

Go:   json.Marshal(obj)
来源：http://bvm.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://ueo.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jfw.zycfv.cn

[K02] JSON 字符串转对象
来源：http://sow.ehwqpu.com

Py:   json.loads(s)
来源：http://zio.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://imw.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://toi.meibo888.top

TS:   JSON.parse(s)
来源：http://pwq.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rbd.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://mwn.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://tfc.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rbt.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://hml.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jao.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bke.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pma.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sdx.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nnw.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kjg.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://lys.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xfc.shuidangran.top

[K04] 读取 JSON 文件
来源：http://cmd.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hbn.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hio.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bhg.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lpd.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ich.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xyr.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ctl.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lfn.hammf.cn

[K05] 深拷贝对象
来源：http://wiv.zhixingplan.top


<!-- 参考信息 -->