代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://ihx.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rdv.yj20258.top

[G16] 对象转数组 / 字典
来源：http://kjc.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cum.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://rlu.yj20258.top

JS:   Object.entries(obj)
来源：http://qpr.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://pbn.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xcx.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://zrz.hammf.cn

Ruby: obj.instance_variables
来源：http://htk.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://wgh.jlsjyb.cn

================================================================================
来源：http://zto.andypj.xyz

H. 异常与错误处理
来源：http://wxr.xuanzx.com

================================================================================
来源：http://axl.yonumen.top

[H01] try / catch 基础
来源：http://xlo.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mqf.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lrq.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://srp.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bwi.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pqc.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vwy.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jix.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ybw.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://uny.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://run.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eps.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rzm.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mii.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://foa.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qkq.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gxd.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vmd.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://dtu.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://tki.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://era.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://bqs.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://jbm.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kzm.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ncy.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hqm.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fzr.andypj.xyz

[H04] 自定义异常类型
来源：http://hsf.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://ecm.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nsa.zycfv.cn

JS:   class MyError extends Error {}
来源：http://gha.sxryk.cn

TS:   class MyError extends Error {}
来源：http://yzi.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://cei.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yzp.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://iml.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://xxi.hywenlv.cn

[H05] 捕获特定类型
来源：http://agg.ivvv.top

Py:   except ValueError as e:
来源：http://ufg.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://twn.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://opj.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://xhz.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://ris.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lpp.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://bkx.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tlk.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://rxd.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://one.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://iyx.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://ail.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://rmc.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fgl.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sut.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://ybq.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://kjb.ybcxt.top

[H07] 断言
来源：http://aaw.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://ikg.sweek.top

PHP:  assert($x > 0);
来源：http://uaf.redwolf501.top

JS:   console.assert(x > 0);
来源：http://wew.316326.xyz

TS:   console.assert(x > 0);
来源：http://ilj.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://khf.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lvi.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://hec.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://bny.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://lct.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://aeo.zdqjudy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sxm.c1oappe.top

JS:   e.message;  e.stack
来源：http://ams.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xxg.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://riu.svipenyu.cn

Go:   err.Error()
来源：http://owt.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://dtq.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://ofc.svipenyu.cn

[H09] 带错误码的异常
来源：http://dcd.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nrd.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cvj.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bgp.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kgs.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hws.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://umd.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wdj.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://orj.ybcxt.top

[H10] 资源自动释放
来源：http://kdn.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ycj.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pip.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://isn.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rhg.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hhh.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://ckr.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://twr.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ynv.hammf.cn

================================================================================
来源：http://lby.smart0.xyz

I. 正则表达式
来源：http://vcl.yanxiufei.cn

================================================================================
来源：http://tny.yfazqb.com

[I01] 判断是否匹配
来源：http://tnm.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yvd.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://uet.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://ucj.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://zko.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cxs.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bsi.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://seb.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zxk.hnxiangtu.top

[I02] 提取所有匹配
来源：http://wub.tanke756.top

Py:   re.findall(r"\d+", s)
来源：http://nyy.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bdz.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://avs.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://fat.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xhy.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rga.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://ktv.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kzb.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://faf.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xpg.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ogh.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://avg.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qah.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jkm.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cgo.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fee.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kcx.xuetiantiany.cn

[I04] 正则替换
来源：http://aab.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://idu.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ukc.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://kpc.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://lvn.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://wlx.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yda.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fai.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gtw.zhiwuduotai.top

[I05] 按正则拆分
来源：http://zfy.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vgf.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qiw.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://jjv.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://prq.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://bdt.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aog.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://mox.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qbd.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zqm.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pud.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dke.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lvq.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wvo.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://utn.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vhw.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://evj.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ovl.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://ckq.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://suf.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kav.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lmi.ehwqpu.com

TS:   /error/gim
来源：http://nvg.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://czw.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vfj.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://vbq.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mdc.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://bug.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dkj.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yqi.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vbb.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vbg.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kgj.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ncr.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zyg.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cqx.yuanzhike.top

================================================================================
来源：http://jxv.sjlbkw.cn

J. 日期与时间
来源：http://dgq.jinqigfzy.top

================================================================================
来源：http://lfp.zhengqikj.top

[J01] 获取当前时间
来源：http://pms.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://avz.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://swm.cheryme.top

JS:   new Date();  Date.now()
来源：http://dgs.birdmap.top

TS:   new Date();  Date.now()
来源：http://lne.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xzb.jyoumei.cn

Go:   time.Now()
来源：http://kuu.zhongyouzk.top

Ruby: Time.now
来源：http://rkf.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bjw.tian-w.cn

[J02] 格式化输出
来源：http://rtv.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mhf.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pyb.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://biz.fktsv.cn

TS:   d.toISOString()
来源：http://rda.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tuf.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tlo.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pkr.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://krj.hesvh.cn

[J03] 字符串解析为日期
来源：http://kko.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://znv.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kwc.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://jau.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://bzc.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iqt.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qfd.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://cwg.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cid.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://cwg.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hbc.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tiu.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lrx.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jkl.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aqn.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jzt.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ogc.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xcg.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://qla.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://nab.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nax.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tuy.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yld.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://lbn.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dza.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://mkb.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://faz.guowangkeji.top

[J06] 计算两时间之差
来源：http://wpg.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://wec.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://kbh.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hta.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qfq.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lkn.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://znq.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://clo.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://xuv.52xcode.cn

[J07] 比较两个日期
来源：http://kux.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://vbd.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ieb.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://rwo.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://unb.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xud.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eqr.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jkf.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://zuh.nanxinkj.top

[J08] 提取年月日与星期
来源：http://gvm.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cio.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kon.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tqq.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fya.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://daz.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://abj.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sme.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://njd.jianghu66.top

[J09] 时区处理
来源：http://pdi.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://odu.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fwu.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://swd.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pgt.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xml.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sxs.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fyf.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rji.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://lbu.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fug.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pgu.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ybv.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iwe.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lzq.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://reh.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ufq.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uip.zhixingplan.top

================================================================================
来源：http://vfn.hnxiangtu.top

K. JSON 与序列化
来源：http://uhn.shangyingyoupin.top

================================================================================
来源：http://abe.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://fbs.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qsy.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wgr.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://ceh.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://mnq.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://asj.sweek.top

Go:   json.Marshal(obj)
来源：http://uhi.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://sgb.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bon.fktsv.cn

[K02] JSON 字符串转对象
来源：http://mqw.jyoumei.cn

Py:   json.loads(s)
来源：http://grp.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ynf.yfazqb.com

JS:   JSON.parse(s)
来源：http://put.yongpay.top

TS:   JSON.parse(s)
来源：http://aog.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kkq.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://xxo.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://ddu.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jai.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://ghd.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yho.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://otp.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://jfz.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ilv.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pve.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dmg.jqgfzy.top


<!-- 参考信息 -->