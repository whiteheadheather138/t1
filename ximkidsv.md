代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://tey.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://isa.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://wdg.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ndl.yonumen.top

PHP:  get_object_vars($obj);
来源：http://ixo.snrcjt.cn

JS:   Object.entries(obj)
来源：http://uxq.fktsv.cn

TS:   Object.entries(obj)
来源：http://vdb.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vhy.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ydf.mhx1999.top

Ruby: obj.instance_variables
来源：http://edp.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://oht.cheryme.top

================================================================================
来源：http://jew.zdbjq.cn

H. 异常与错误处理
来源：http://okb.fanxiaobao.xyz

================================================================================
来源：http://ssv.xinyue.icu

[H01] try / catch 基础
来源：http://bjd.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zac.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tds.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yky.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tcl.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pbt.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ioy.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iha.smart0.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://axc.sysykeji.top

[H02] finally / ensure 收尾
来源：http://hgd.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qgm.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uwl.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://znm.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tcs.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://smg.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xnq.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://nyi.hammf.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://evs.52xcode.cn

[H03] 主动抛出异常
来源：http://gzb.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://ffl.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dao.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://rrm.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://elp.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zfe.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lom.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vio.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://goq.yuanzhike.top

[H04] 自定义异常类型
来源：http://zyg.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://awc.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kwu.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://wsg.yueranfly.top

TS:   class MyError extends Error {}
来源：http://jjb.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://gwf.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://inb.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://kaf.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://omv.guannengcc.top

[H05] 捕获特定类型
来源：http://qqr.zycfv.cn

Py:   except ValueError as e:
来源：http://yxt.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vcc.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://rbr.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://iva.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://coa.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fxe.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://xpb.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bam.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://tok.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://phv.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bdf.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://eys.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://nqx.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ppb.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://hgl.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://qym.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://nlc.yuanzhike.top

[H07] 断言
来源：http://nvd.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://cfv.yongpay.top

PHP:  assert($x > 0);
来源：http://twi.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://tkq.sxryk.cn

TS:   console.assert(x > 0);
来源：http://cml.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://lcj.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xma.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://jcm.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://lmj.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://sze.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://jwt.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbb.sxryk.cn

JS:   e.message;  e.stack
来源：http://mdw.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://psl.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://crw.quarkkingdee.top

Go:   err.Error()
来源：http://hql.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://zcs.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://mln.hammf.cn

[H09] 带错误码的异常
来源：http://pam.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cxd.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yex.fzhhl.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blg.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wtf.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://idu.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kdt.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://ztu.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xpl.wangshuangyany.cn

[H10] 资源自动释放
来源：http://hpj.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lfb.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://clv.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qqo.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cmo.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://twd.shzxlz.cn

Go:   defer f.Close()
来源：http://txp.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iyu.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lbk.fzhhl.top

================================================================================
来源：http://whi.sufxvd.cn

I. 正则表达式
来源：http://ofj.hnqzz.top

================================================================================
来源：http://aki.zycfv.cn

[I01] 判断是否匹配
来源：http://wnl.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ykj.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://qfm.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://ciw.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://wfx.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ayi.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oyt.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://vxm.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xcl.redwolf501.top

[I02] 提取所有匹配
来源：http://sts.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://vkr.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://row.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vtp.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://ygp.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fzl.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wkx.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://esa.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wqm.nanxinkj.top

[I03] 提取捕获分组
来源：http://uev.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ybl.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://puy.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://imu.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gue.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yhn.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pzk.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qri.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ubm.jyoumei.cn

[I04] 正则替换
来源：http://wnt.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xvd.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rve.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://udy.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://wda.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://irh.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://grr.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dtl.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xnz.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://zew.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ezv.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jpp.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://ecq.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://jkv.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://tpd.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ije.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://vol.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://luz.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://osl.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yxn.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aaq.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aix.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gde.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hmv.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lji.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rmr.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lxt.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://anj.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mri.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://txm.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cjb.nanxinkj.top

TS:   /error/gim
来源：http://jcs.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ake.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://deh.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://ddg.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gud.zhengqikj.top

[I08] 贪婪与非贪婪匹配
来源：http://zth.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://icp.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hqw.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qze.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://miq.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ihy.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sxu.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vfo.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iqw.52xcode.cn

================================================================================
来源：http://bty.jinghuilouyu.cn

J. 日期与时间
来源：http://dfi.ctjpmb.com

================================================================================
来源：http://dzy.hnqzz.top

[J01] 获取当前时间
来源：http://qgl.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xue.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ebn.wangdashe.top

JS:   new Date();  Date.now()
来源：http://goq.yongpay.top

TS:   new Date();  Date.now()
来源：http://lvh.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pyx.andypj.xyz

Go:   time.Now()
来源：http://eyl.fktsv.cn

Ruby: Time.now
来源：http://ast.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zpk.shuidangran.top

[J02] 格式化输出
来源：http://ntv.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gng.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kht.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wcj.daxiang520.top

TS:   d.toISOString()
来源：http://gra.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nbm.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nwm.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zaa.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wgm.daxiang520.top

[J03] 字符串解析为日期
来源：http://yue.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mhk.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://twy.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://oyg.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://fby.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mnx.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hcm.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://gci.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hyv.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://lwq.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gcw.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nxu.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://piq.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rte.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lny.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eeg.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dwl.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spi.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://ruf.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://cyr.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xuu.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zjl.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eft.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://hmt.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sbe.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://avd.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://usp.redwolf501.top

[J06] 计算两时间之差
来源：http://feg.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://hjq.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://kex.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cim.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bdv.bbcook.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zlu.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://dbg.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://rbm.mhx1999.top

C#:   (end - start).TotalSeconds
来源：http://bce.zhixingplan.top

[J07] 比较两个日期
来源：http://oka.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://zdp.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pae.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lgi.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://eij.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fym.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://agd.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://dkf.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://hsw.xuanzx.com

[J08] 提取年月日与星期
来源：http://xop.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://loc.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zht.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mcl.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://usy.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gbh.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://grr.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vcu.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ntq.yonumen.top

[J09] 时区处理
来源：http://anj.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ktr.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pry.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cpx.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lcx.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://woq.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vdk.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ryv.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vnm.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://jgx.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dhz.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sig.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bsn.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lpn.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rfe.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oul.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yzf.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://snq.ydjk.org.cn

================================================================================
来源：http://ckf.yj20258888.top

K. JSON 与序列化
来源：http://oeo.jqgufenzy.top

================================================================================
来源：http://cfp.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://tgx.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yil.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ozw.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://phm.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://znn.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://enq.wangdashe.top

Go:   json.Marshal(obj)
来源：http://hkl.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://odg.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fxh.fzhhl.top

[K02] JSON 字符串转对象
来源：http://zaq.guowangkeji.top

Py:   json.loads(s)
来源：http://kxv.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zle.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://knq.nwbrower.top

TS:   JSON.parse(s)
来源：http://osz.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://myc.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://ltb.andypj.xyz

Ruby: JSON.parse(s)
来源：http://ezi.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pml.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://med.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://imy.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vjj.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://adn.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ead.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://scb.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lbu.52xcode.cn


<!-- 参考信息 -->