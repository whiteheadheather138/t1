代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://zhn.havefunace.top

Ruby: obj.instance_variables
来源：http://zor.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://hwm.daria6918.cn

================================================================================
来源：http://glm.zhijiandao.cn

H. 异常与错误处理
来源：http://mkh.sweek.top

================================================================================
来源：http://vge.haohaochexian.top

[H01] try / catch 基础
来源：http://vrd.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yam.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zfb.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yld.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vam.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://exp.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aba.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgf.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ynu.yj20258888.top

[H02] finally / ensure 收尾
来源：http://wpa.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://wuo.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bfc.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cwl.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cuv.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bhj.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wzi.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cvy.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmn.nanxuanxn.top

[H03] 主动抛出异常
来源：http://bdg.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://fcn.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bdi.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://rrx.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://ifz.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uyc.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gjp.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qyw.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://mkh.iojbl.cn

[H04] 自定义异常类型
来源：http://wbv.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://aav.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xvo.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://tvz.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://xto.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://kbj.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eqo.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://mkd.yonumen.top

C#:   class MyException : Exception {}
来源：http://abp.pycfn.com

[H05] 捕获特定类型
来源：http://lnu.xziqi.cn

Py:   except ValueError as e:
来源：http://hun.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uwi.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://efd.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://lfn.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://nvf.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ltj.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://mtb.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hcz.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://qnk.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://tdh.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://hsy.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jbf.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://ntu.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://isk.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yaf.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://ndt.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://xxh.tian-w.cn

[H07] 断言
来源：http://aue.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://snv.ydzc1.top

PHP:  assert($x > 0);
来源：http://xux.ivvv.top

JS:   console.assert(x > 0);
来源：http://qau.yj20258.top

TS:   console.assert(x > 0);
来源：http://ymk.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://ola.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sic.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://npf.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://mmi.chenlongwang.top

[H08] 获取错误信息与堆栈
来源：http://klq.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://aoy.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fpj.zycfv.cn

JS:   e.message;  e.stack
来源：http://kqa.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lvd.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://wyl.bjfxy.top

Go:   err.Error()
来源：http://gyh.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://igq.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://mzr.cqqwz.cn

[H09] 带错误码的异常
来源：http://mwk.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rfq.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rij.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ecj.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://frk.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cfp.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hbg.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://mkz.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pgh.cdnleiting.top

[H10] 资源自动释放
来源：http://hch.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ppz.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ked.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fbh.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kgo.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://emd.ivvv.top

Go:   defer f.Close()
来源：http://xky.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gmp.cashguo.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bvv.yueranfly.top

================================================================================
来源：http://fro.zdqjudy.top

I. 正则表达式
来源：http://jwk.zdqjudy.top

================================================================================
来源：http://bzr.sweek.top

[I01] 判断是否匹配
来源：http://fzw.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oqw.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://wmq.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://ktr.yj20258.top

TS:   /\d+/.test(s)
来源：http://xtv.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mpc.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wbi.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://xkg.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vbc.hfpthk.cn

[I02] 提取所有匹配
来源：http://ull.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://eca.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://veb.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vdu.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://uus.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jwv.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://btw.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://rnp.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lod.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://hxv.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gws.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uym.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jgi.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eyf.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nry.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uyc.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fkn.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ngn.chenlongwang.top

[I04] 正则替换
来源：http://wjq.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://dho.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rop.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ljx.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://lyc.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xyh.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yaa.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ooq.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kkq.wangdashe.top

[I05] 按正则拆分
来源：http://eqa.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eop.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lqj.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://xin.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://xun.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://evc.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gkg.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://btd.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fpt.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://flk.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ilk.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hbn.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://imb.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xvr.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://san.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://djj.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mej.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pyh.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://tvx.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tem.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wlz.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jdk.birdmap.top

TS:   /error/gim
来源：http://vxh.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vmg.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://irb.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://sjb.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vos.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://lov.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dog.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hng.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xdl.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vmr.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://hac.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://num.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vhw.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ndq.hnxiangtu.top

================================================================================
来源：http://pbe.hywenlv.cn

J. 日期与时间
来源：http://uxy.gaohongyu789.top

================================================================================
来源：http://ngx.svipenyu.cn

[J01] 获取当前时间
来源：http://clc.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://ydr.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wgp.yongpay.top

JS:   new Date();  Date.now()
来源：http://wmm.tian-w.cn

TS:   new Date();  Date.now()
来源：http://tjg.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pez.hnxiangtu.top

Go:   time.Now()
来源：http://yiq.cucudq.cn

Ruby: Time.now
来源：http://vvx.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ezb.pengpengdd.cyou

[J02] 格式化输出
来源：http://kbe.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pof.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fiv.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ccv.fktsv.cn

TS:   d.toISOString()
来源：http://ktq.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://deu.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mgn.jqgufenzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lrh.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wea.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://omo.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zkc.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gpv.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://tvn.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://aek.pengpengdd.cyou

Java: LocalDate.parse("2024-01-02")
来源：http://ico.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jxp.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://mgu.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gnt.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://kah.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://crh.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nam.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zkg.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lub.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dqd.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hat.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mrw.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dus.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://foa.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://rvs.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jfu.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qvm.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nul.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://ppf.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ioj.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://tql.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://etw.xinyue.icu

[J06] 计算两时间之差
来源：http://hrc.uphjek.com

Py:   (end - start).total_seconds()
来源：http://stk.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://qmd.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qta.52xcode.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yyu.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://ehs.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://ofa.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://eax.sweek.top

C#:   (end - start).TotalSeconds
来源：http://qgs.cheryme.top

[J07] 比较两个日期
来源：http://dtt.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://cam.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qdq.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://nbb.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://waf.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://imt.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jti.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://tig.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://sic.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://wmk.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://owd.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jrl.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ohm.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qhg.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://exz.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yzi.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gzj.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://npj.ivvv.top

[J09] 时区处理
来源：http://mek.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mpj.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gis.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lbu.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blh.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jbz.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pyf.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pdc.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oxu.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://ekz.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xnn.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zks.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ykp.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mut.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yjc.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ads.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://egu.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cxp.hammf.cn

================================================================================
来源：http://sww.aibaodan.cn

K. JSON 与序列化
来源：http://hhv.ppjwa.cn

================================================================================
来源：http://dce.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://css.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lbi.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jlu.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://xrf.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://zkv.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vrc.fktsv.cn

Go:   json.Marshal(obj)
来源：http://wst.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://cut.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://sjv.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://phb.jlsjyb.cn

Py:   json.loads(s)
来源：http://jgk.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kah.chenlongwang.top

JS:   JSON.parse(s)
来源：http://ikm.yonumen.top

TS:   JSON.parse(s)
来源：http://wtd.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ewc.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://hba.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://yoi.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://igv.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://pmt.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://evm.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aen.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://obh.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jpo.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sxx.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://arp.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uas.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://syw.xylfe.cn

[K04] 读取 JSON 文件
来源：http://wow.sjlbkw.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gtg.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kxr.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ihx.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbd.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uxx.yuanzhike.top


<!-- 参考信息 -->