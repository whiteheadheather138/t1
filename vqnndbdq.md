代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://uxr.cqqwz.cn

Ruby: obj.instance_variables
来源：http://ikm.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://hpe.cucudq.cn

================================================================================
来源：http://xbr.svipenyu.cn

H. 异常与错误处理
来源：http://nsy.xingfuxueyuan.xyz

================================================================================
来源：http://lhv.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://fig.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dju.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cyj.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ieg.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sec.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vch.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wtt.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ddc.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rnw.yfazqb.com

[H02] finally / ensure 收尾
来源：http://bbh.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fog.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mej.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mzk.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://erj.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://nuk.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hmr.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://piq.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://wsa.sysykeji.top

[H03] 主动抛出异常
来源：http://gdk.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://tuk.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ikj.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://fgm.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://jiq.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lpx.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qkz.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://srr.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://plo.svipenyu.cn

[H04] 自定义异常类型
来源：http://tfq.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://wmz.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hao.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://iqn.hammf.cn

TS:   class MyError extends Error {}
来源：http://gck.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://uvl.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://btp.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://nhg.gzhubu.top

C#:   class MyException : Exception {}
来源：http://fqz.jianghu66.top

[H05] 捕获特定类型
来源：http://zsy.vqdsnc.cn

Py:   except ValueError as e:
来源：http://wzt.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lcf.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://rbg.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://rpe.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://wtc.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cbb.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://iav.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gry.jinyuanbaomall.cn

[H06] 可选值 / 空值安全访问
来源：http://dzm.yj20258.top

Py:   value = d.get("k") or default
来源：http://cwt.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://wgz.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wmu.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fbt.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wea.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qsg.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://vwg.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://pzu.fengsongda.top

[H07] 断言
来源：http://lpm.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://rzf.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://tyq.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://rhj.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://dpo.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://wue.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://frb.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://kyd.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://dpa.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://piy.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://rgg.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fno.birdmap.top

JS:   e.message;  e.stack
来源：http://jpa.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://phb.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hjb.vqdsnc.cn

Go:   err.Error()
来源：http://ptf.sweek.top

Ruby: e.message;  e.backtrace
来源：http://xpp.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://eho.yonumen.top

[H09] 带错误码的异常
来源：http://cer.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rws.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jgn.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rnv.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://unq.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zwm.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ict.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uqw.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xna.guowangkeji.top

[H10] 资源自动释放
来源：http://ovq.fktsv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mmj.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vsv.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wpd.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ruz.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sga.daria6918.cn

Go:   defer f.Close()
来源：http://fjd.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rkj.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wkm.ydjk.org.cn

================================================================================
来源：http://jta.sweek.top

I. 正则表达式
来源：http://jbv.yongpay.top

================================================================================
来源：http://hai.ctjpmb.com

[I01] 判断是否匹配
来源：http://qhf.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mvb.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lej.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://nbe.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://lhm.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tke.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ivz.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://nbq.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tcg.dianchejie.cn

[I02] 提取所有匹配
来源：http://tqe.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://wwp.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mvu.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cux.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://fzt.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xhh.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sgw.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://kle.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tht.ehwqpu.com

[I03] 提取捕获分组
来源：http://uhj.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wqz.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jui.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tdy.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://knb.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cwi.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dch.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bkp.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xcx.meibo888.top

[I04] 正则替换
来源：http://vjg.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://keo.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dav.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://zts.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vho.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://yyc.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aiv.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://usg.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qai.fzhhl.top

[I05] 按正则拆分
来源：http://lmo.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://efk.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rxc.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://dcg.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://njw.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://ucj.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fmj.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://lee.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xnk.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kza.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cnm.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bnc.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyq.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gef.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nbk.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fap.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gho.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jbi.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://irp.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yyo.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nsi.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zws.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://gsu.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zlx.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fep.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://fke.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mwr.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://tkk.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://azb.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fnf.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qqb.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://elo.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zfk.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dik.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wbb.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gtx.yuanzhike.top

================================================================================
来源：http://qnf.iojbl.cn

J. 日期与时间
来源：http://ezq.ybcxt.top

================================================================================
来源：http://gte.gaohongyu789.top

[J01] 获取当前时间
来源：http://ryb.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kgq.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aht.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://jvm.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://cfy.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lkk.jqgufenzy.top

Go:   time.Now()
来源：http://hyp.zhongyouzk.top

Ruby: Time.now
来源：http://nkb.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mjd.jqgfzy.top

[J02] 格式化输出
来源：http://biy.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://niq.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oud.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qnu.daxiang520.top

TS:   d.toISOString()
来源：http://fzu.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gtn.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fwb.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ebi.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://okd.epnwcf.com

[J03] 字符串解析为日期
来源：http://msl.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ont.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pae.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://vaq.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://bnd.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://ovz.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fal.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://uco.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://quq.redwolf501.top

[J04] 时间戳与日期互转
来源：http://szk.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://npp.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dvc.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pce.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wff.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xot.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xmm.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mzh.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lpe.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://dbx.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://rpd.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://wth.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nyw.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zbr.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://rag.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pqn.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://frx.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xle.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://qzm.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://grq.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://aiy.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tvv.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jzv.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://twr.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://xqs.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://zgw.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://ivx.svipenyu.cn

[J07] 比较两个日期
来源：http://hzu.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://cgo.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ojx.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://eop.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kzw.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jps.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://prg.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sba.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://owh.yj20258888.top

[J08] 提取年月日与星期
来源：http://isi.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bpw.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ldo.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jci.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kei.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yfs.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qmo.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pbq.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://feu.cqqwz.cn

[J09] 时区处理
来源：http://xgu.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cgv.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nwd.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lza.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://spg.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qim.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qpb.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mkg.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://brb.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://pxb.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tvh.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pkg.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nvi.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://asf.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bbl.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://axo.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wdk.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://msi.shangyingyoupin.top

================================================================================
来源：http://szu.jinghuilouyu.cn

K. JSON 与序列化
来源：http://dho.zhongyouzk.top

================================================================================
来源：http://ivh.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://jmj.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ike.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ggn.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://djx.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://bxh.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lyi.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://hsd.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://eln.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qrj.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://ztk.fehbvm.com

Py:   json.loads(s)
来源：http://ijl.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pzr.316326.xyz

JS:   JSON.parse(s)
来源：http://fpo.zdbjq.cn

TS:   JSON.parse(s)
来源：http://mrr.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://flk.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://vvg.cheryme.top

Ruby: JSON.parse(s)
来源：http://bcx.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xpb.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://tdm.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kam.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dyi.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zvb.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zpe.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uvg.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mjd.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lyf.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jnx.zhongyouzk.top

[K04] 读取 JSON 文件
来源：http://wdt.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jae.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ksm.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kgf.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tof.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://krg.ivvv.top


<!-- 参考信息 -->