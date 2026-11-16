代发 wailian999

PHP:  get_object_vars($obj);
来源：http://xpc.ybcxt.top

JS:   Object.entries(obj)
来源：http://nti.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://ytt.yj20258.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tor.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lek.shuidangran.top

Ruby: obj.instance_variables
来源：http://jhu.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://bfg.zhixingplan.top

================================================================================
来源：http://zpl.fehbvm.com

H. 异常与错误处理
来源：http://kkb.jinyuanbaomall.cn

================================================================================
来源：http://kuw.meibo888.top

[H01] try / catch 基础
来源：http://aui.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xkd.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xtd.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mzz.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sjm.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vyc.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bzt.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kjr.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lpl.yongpay.top

[H02] finally / ensure 收尾
来源：http://wzn.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lba.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jzq.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://njq.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ruj.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://mho.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wgh.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://vnj.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hab.bbcook.cn

[H03] 主动抛出异常
来源：http://wee.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://xgq.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dcs.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://bgx.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://xpq.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eez.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://est.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ztq.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://plb.sweek.top

[H04] 自定义异常类型
来源：http://dkf.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://hpo.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jhv.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://dni.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://jte.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://spd.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://edu.sweek.top

Ruby: class MyError < StandardError; end
来源：http://jew.andypj.xyz

C#:   class MyException : Exception {}
来源：http://djs.snrcjt.cn

[H05] 捕获特定类型
来源：http://eyk.jqgufenzy.top

Py:   except ValueError as e:
来源：http://gfs.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hjv.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://sst.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://fnp.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://bey.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mif.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://tqp.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lhz.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://sus.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://hds.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://jsh.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gbf.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wtx.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rrb.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ptp.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://fyw.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://hbz.jinyuanbaomall.cn

[H07] 断言
来源：http://tkt.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://rhr.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://yym.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://bjo.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://kzd.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://avg.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ely.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pzq.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://ikw.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://obx.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://nqv.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zho.0kj1m.cn

JS:   e.message;  e.stack
来源：http://wnn.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dcx.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hkx.jqgufenzy.top

Go:   err.Error()
来源：http://uys.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://joh.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://xsm.zdbjq.cn

[H09] 带错误码的异常
来源：http://xrj.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fvi.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://knv.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eur.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mgd.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vup.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jqh.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dpe.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://qdx.zhoulong.xyz

[H10] 资源自动释放
来源：http://dps.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xvn.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fxp.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uir.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tso.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gml.nanxinkj.top

Go:   defer f.Close()
来源：http://rkw.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mss.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rlb.jiagoushi.top

================================================================================
来源：http://dzz.tianlin.xyz

I. 正则表达式
来源：http://ffl.cqqwz.cn

================================================================================
来源：http://mww.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://pfz.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dln.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xpe.yj20258.top

JS:   /\d+/.test(s)
来源：http://vew.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://qxs.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ldn.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nrx.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://uyi.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://chu.yfazqb.com

[I02] 提取所有匹配
来源：http://kni.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://vjc.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ucc.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://egi.birdmap.top

TS:   s.match(/\d+/g)
来源：http://tjv.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cbg.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://got.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://ddd.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mxy.zdbjq.cn

[I03] 提取捕获分组
来源：http://ltj.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://huq.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zll.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sux.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rdd.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vhy.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://awi.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qpx.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jzx.vqdsnc.cn

[I04] 正则替换
来源：http://sxe.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cfz.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gce.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://szn.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://pme.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://ztz.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rvh.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hmv.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lrw.zycfv.cn

[I05] 按正则拆分
来源：http://gqc.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lki.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ubb.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://tch.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://nkr.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://anx.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lzd.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://iij.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ptx.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ulj.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://euq.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xan.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rmu.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://abx.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yne.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lla.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zfb.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lfn.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://bcz.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ubc.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rsv.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oya.uphjek.com

TS:   /error/gim
来源：http://xov.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qmd.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qkj.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://zes.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vza.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://eqg.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hig.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ylq.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ryl.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tjl.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wip.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xxk.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://twx.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://whk.svipenyu.cn

================================================================================
来源：http://wqu.nwbrower.top

J. 日期与时间
来源：http://ckg.fanxiaobao.xyz

================================================================================
来源：http://iqg.jianghu66.top

[J01] 获取当前时间
来源：http://rwg.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bqs.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ody.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://esl.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://dbo.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ecy.jyoumei.cn

Go:   time.Now()
来源：http://xas.ydjk.org.cn

Ruby: Time.now
来源：http://lsz.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lzw.cqqwz.cn

[J02] 格式化输出
来源：http://exz.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mau.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rxu.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mgv.cucudq.cn

TS:   d.toISOString()
来源：http://bsx.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gbr.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dgq.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tdw.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dbx.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://atm.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://isi.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpg.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://gpd.yongpay.top

TS:   new Date("2024-01-02")
来源：http://fus.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://cur.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dft.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://grt.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ofx.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://jqw.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fpc.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dvr.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eee.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yla.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fxf.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mkn.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://txx.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pwu.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://cjs.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://zgy.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jyx.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://piw.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cjx.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://nkm.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gfh.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://ewb.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://xwn.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://fes.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://iow.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://yht.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ayg.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uta.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://ebs.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://xax.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://kji.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://pei.ydjk.org.cn

[J07] 比较两个日期
来源：http://iql.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://hsr.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xvz.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://tir.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://cdm.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sjl.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vcr.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kty.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://mqa.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://few.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lrb.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ltu.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gay.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://okd.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jor.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cca.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hge.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ztg.tian-w.cn

[J09] 时区处理
来源：http://abg.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vpp.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xdc.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gns.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pfv.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qzl.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ajh.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wxs.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bzk.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://wpd.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zjz.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xck.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://udi.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iay.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pnv.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zap.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ogo.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mkm.havefunace.top

================================================================================
来源：http://aaf.yuxming.cn

K. JSON 与序列化
来源：http://qkt.9152youxi.cn

================================================================================
来源：http://bxl.sweek.top

[K01] 对象转 JSON 字符串
来源：http://wbk.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uco.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dtb.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://qxe.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://als.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ase.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://xke.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://cnh.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iza.fzhhl.top

[K02] JSON 字符串转对象
来源：http://tyk.pycfn.com

Py:   json.loads(s)
来源：http://tjn.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bdz.ppjwa.cn

JS:   JSON.parse(s)
来源：http://ovg.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://uol.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xnc.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://hos.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://kiv.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ina.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://xwi.yuanzhike.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qxp.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rau.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kqr.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cts.tian-w.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dod.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wjp.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://weo.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://muy.xylfe.cn

[K04] 读取 JSON 文件
来源：http://vnr.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xjn.chenlongwang.top


<!-- 参考信息 -->