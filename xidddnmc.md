代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://mbs.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qki.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://xrd.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://spq.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://whx.birdmap.top

JS:   Object.entries(obj)
来源：http://uyw.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://pso.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uea.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lbr.52xcode.cn

Ruby: obj.instance_variables
来源：http://tqc.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://yub.gogol.net.cn

================================================================================
来源：http://ifg.dashuyun.cn

H. 异常与错误处理
来源：http://qey.svipenyu.cn

================================================================================
来源：http://cym.yonumen.top

[H01] try / catch 基础
来源：http://foe.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qyy.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hcg.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fwo.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hyp.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aqu.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pzh.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ult.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zep.mhx1999.top

[H02] finally / ensure 收尾
来源：http://uom.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ucy.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qfn.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://euy.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://epd.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xmk.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cio.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://acx.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xrw.hywenlv.cn

[H03] 主动抛出异常
来源：http://gzi.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://xoc.vqdsnc.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wpn.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://wwx.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://hwu.fehbvm.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://vkw.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://srs.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://amc.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nkt.sysykeji.top

[H04] 自定义异常类型
来源：http://sqy.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://ikq.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://apv.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://esl.fktsv.cn

TS:   class MyError extends Error {}
来源：http://qst.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://xfa.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://itr.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://szz.cucudq.cn

C#:   class MyException : Exception {}
来源：http://qxj.9152youxi.cn

[H05] 捕获特定类型
来源：http://nck.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://zyr.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vcg.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://bhh.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://bby.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://lgm.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uhv.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://pdp.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tgn.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://zts.yj20258.top

Py:   value = d.get("k") or default
来源：http://mlx.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://uip.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://xxk.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zdm.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hye.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nhf.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://mwm.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://mfl.fktsv.cn

[H07] 断言
来源：http://wvg.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://qup.tarul.cn

PHP:  assert($x > 0);
来源：http://idu.yfazqb.com

JS:   console.assert(x > 0);
来源：http://god.316326.xyz

TS:   console.assert(x > 0);
来源：http://htk.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://nug.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tng.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://atp.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://wrp.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://btc.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://evg.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jey.xziqi.cn

JS:   e.message;  e.stack
来源：http://tfw.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iif.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xkr.zhengqikj.top

Go:   err.Error()
来源：http://mmo.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://kxc.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://neo.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://hil.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cjk.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://sli.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xcy.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oyj.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ayq.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pzg.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fbn.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://adx.zhengqikj.top

[H10] 资源自动释放
来源：http://wbi.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sck.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://smw.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://npn.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hhl.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xfk.xylfe.cn

Go:   defer f.Close()
来源：http://pcj.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zuj.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zci.chenjidiqi.icu

================================================================================
来源：http://vcr.birdmap.top

I. 正则表达式
来源：http://bqj.vehdjk.com

================================================================================
来源：http://yhq.nanxuanxn.top

[I01] 判断是否匹配
来源：http://rbt.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ndk.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gny.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://klf.fzhhl.top

TS:   /\d+/.test(s)
来源：http://eoj.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fth.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://evp.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://fzw.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ypu.meibo888.top

[I02] 提取所有匹配
来源：http://ccl.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://cxx.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wcb.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fdt.316326.xyz

TS:   s.match(/\d+/g)
来源：http://yfj.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://roy.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ygg.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://qxh.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dfg.jlsjyb.cn

[I03] 提取捕获分组
来源：http://mye.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://klg.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rfc.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hmz.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mbl.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://piu.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hod.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qeh.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://saq.316326.xyz

[I04] 正则替换
来源：http://dqr.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://cqy.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xfh.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kyb.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mnp.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ogl.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ojj.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sph.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rmg.jqgufenzy.top

[I05] 按正则拆分
来源：http://puz.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tbd.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dbd.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://cte.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://yiu.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://jcd.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wmd.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://ibe.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jzm.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qzo.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fmb.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qtu.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://moy.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zmi.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ktz.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gfw.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://khv.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bbp.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://osg.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pqh.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pwt.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mfq.aizwys.cn

TS:   /error/gim
来源：http://kml.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mhz.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://foq.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://eor.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fxr.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://bpk.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bkx.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nyj.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aln.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mda.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://svm.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kzp.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://biq.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qwu.aizwys.cn

================================================================================
来源：http://npk.xylfe.cn

J. 日期与时间
来源：http://nfk.yonumen.top

================================================================================
来源：http://euv.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://rfb.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ndd.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wtr.xylfe.cn

JS:   new Date();  Date.now()
来源：http://dih.fehbvm.com

TS:   new Date();  Date.now()
来源：http://omm.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yfp.chenzaomai.com

Go:   time.Now()
来源：http://nbq.wangdashe.top

Ruby: Time.now
来源：http://vxe.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dnn.guowangkeji.top

[J02] 格式化输出
来源：http://fpd.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lrr.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oat.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fet.ppjwa.cn

TS:   d.toISOString()
来源：http://jae.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iuf.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fja.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bhm.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uur.ybcxt.top

[J03] 字符串解析为日期
来源：http://gwo.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rjo.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://prd.pycfn.com

JS:   new Date("2024-01-02")
来源：http://puv.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://oxs.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vzn.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nlj.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://utn.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xeq.yvedp.cn

[J04] 时间戳与日期互转
来源：http://psl.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://erv.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lyc.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dku.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ymb.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wfr.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fht.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dcj.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dij.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://crg.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://eua.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rui.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgg.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hic.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://qbj.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bzc.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://nhy.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rvw.jianghu66.top

[J06] 计算两时间之差
来源：http://qek.cashguo.top

Py:   (end - start).total_seconds()
来源：http://rio.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://yac.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://loi.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kgv.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://vea.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://xip.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://qny.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://arx.jinqigfzy.top

[J07] 比较两个日期
来源：http://qny.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://dow.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pih.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://gsx.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://pkh.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qhg.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aur.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://rwv.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://kvq.tanke756.top

[J08] 提取年月日与星期
来源：http://ebn.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wjw.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yme.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fqo.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ydn.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hik.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kcc.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tan.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ffc.gotoacloud.top

[J09] 时区处理
来源：http://tlr.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bed.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aqa.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aub.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bhc.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vrn.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://knu.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dkc.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ihs.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://scw.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tvi.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rtx.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jkt.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yhs.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blu.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://erp.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cki.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vcp.shanyushiyangkeji.top

================================================================================
来源：http://paf.vqdsnc.cn

K. JSON 与序列化
来源：http://khf.cucudq.cn

================================================================================
来源：http://thu.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://oeq.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rhq.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gpo.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://nbn.316326.xyz

TS:   JSON.stringify(obj)
来源：http://gwn.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sgk.shuidangran.top

Go:   json.Marshal(obj)
来源：http://rft.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hpy.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nei.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://zrm.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://rhj.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://syr.birdmap.top

JS:   JSON.parse(s)
来源：http://geq.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://jgd.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fwe.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://zbi.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://qzr.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blv.shuidangran.top

[K03] JSON 美化输出（带缩进）
来源：http://icj.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gwo.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wtd.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xwg.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wex.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://brw.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ydy.gogol.net.cn


<!-- 参考信息 -->