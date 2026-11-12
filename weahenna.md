代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://qwq.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nnj.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://gvq.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pyb.yongpay.top

PHP:  get_object_vars($obj);
来源：http://uzu.tarul.cn

JS:   Object.entries(obj)
来源：http://wws.fengsongda.top

TS:   Object.entries(obj)
来源：http://ivc.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://plo.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jah.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://vhz.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://wtn.yangfankeji.com

================================================================================
来源：http://kcr.birdmap.top

H. 异常与错误处理
来源：http://hzh.zhongyouzk.top

================================================================================
来源：http://ssu.nwbrower.top

[H01] try / catch 基础
来源：http://fsj.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://idd.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kzh.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oyk.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://peh.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://llj.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://drz.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sfd.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nhp.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://uoz.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vpf.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xel.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mpj.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://axn.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://env.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://joa.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://wba.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://urt.tarul.cn

[H03] 主动抛出异常
来源：http://pvi.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://ysy.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gqb.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://kbo.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://xlp.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vbb.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://htp.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sfx.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://ufg.epnwcf.com

[H04] 自定义异常类型
来源：http://dfi.ivvv.top

Py:   class MyError(Exception): pass
来源：http://iyl.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://usk.xziqi.cn

JS:   class MyError extends Error {}
来源：http://itx.iojbl.cn

TS:   class MyError extends Error {}
来源：http://djx.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://pmb.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://asl.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://zea.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://pkf.hywenlv.cn

[H05] 捕获特定类型
来源：http://mjt.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://vjc.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eca.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://rja.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://tds.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://igd.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://okn.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://iga.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dnn.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://koa.daxiang520.top

Py:   value = d.get("k") or default
来源：http://esu.havefunace.top

PHP:  $v = $d["k"] ?? null;
来源：http://ouo.zhaomingkeji.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://khn.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hoz.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cty.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xpl.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://eon.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://mlx.c1oappe.top

[H07] 断言
来源：http://pdj.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://clv.xylfe.cn

PHP:  assert($x > 0);
来源：http://ocb.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://ond.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://enk.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://mcl.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lws.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ndh.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://ozt.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://wgr.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://bax.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rso.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://jwf.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://etv.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zdr.haohaochexian.top

Go:   err.Error()
来源：http://vyp.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://fai.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://wzu.sjlbkw.cn

[H09] 带错误码的异常
来源：http://wxf.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://roo.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sqw.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xhg.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zhn.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xwo.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kyo.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pvq.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://psc.hysaishi.cn

[H10] 资源自动释放
来源：http://gur.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zer.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pfi.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xzn.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hwj.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tgw.tarul.cn

Go:   defer f.Close()
来源：http://xty.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lep.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eoe.yueranfly.top

================================================================================
来源：http://wln.zdqjudy.top

I. 正则表达式
来源：http://vfk.yvedp.cn

================================================================================
来源：http://zyu.zdqjudy.top

[I01] 判断是否匹配
来源：http://phj.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mqd.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yah.yonumen.top

JS:   /\d+/.test(s)
来源：http://bsx.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://wxv.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jfz.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kzn.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://jyf.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://asg.cqqwz.cn

[I02] 提取所有匹配
来源：http://oln.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://jrc.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zll.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ufi.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://gzh.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oqu.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bsm.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://wcl.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yed.zhijiandao.cn

[I03] 提取捕获分组
来源：http://vln.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wlr.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ldm.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jsr.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nje.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ioh.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uxs.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fcb.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mhl.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://fuv.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lhk.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qwe.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ibb.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hcp.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://aff.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ssn.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kyg.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hhk.jlsjyb.cn

[I05] 按正则拆分
来源：http://feo.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jnb.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sfm.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://gng.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://ocv.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://sgp.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wke.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://knh.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yrn.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wqg.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xar.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lzh.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tjw.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://klq.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://npc.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zog.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://irt.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://trw.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://gri.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xif.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://czl.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bkq.jinyuanbaomall.cn

TS:   /error/gim
来源：http://hmo.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://llh.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://glj.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://cdl.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fuy.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://nqj.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jvf.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hct.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uey.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lzx.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hmj.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://igw.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xpz.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tiz.shzxlz.cn

================================================================================
来源：http://wxg.fengsongda.top

J. 日期与时间
来源：http://psw.sufxvd.cn

================================================================================
来源：http://azf.sweek.top

[J01] 获取当前时间
来源：http://vlw.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tcr.hammf.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://psp.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://mvu.yongpay.top

TS:   new Date();  Date.now()
来源：http://aso.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cvv.tianlin.xyz

Go:   time.Now()
来源：http://fww.andypj.xyz

Ruby: Time.now
来源：http://pgk.hnxiangtu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ozt.gaohongyu789.top

[J02] 格式化输出
来源：http://sfn.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqi.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ppp.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ven.hongshengwenyu.top

TS:   d.toISOString()
来源：http://xqt.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://add.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mxp.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ney.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mni.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://frs.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mpm.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xtk.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://mmq.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://kui.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://sby.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xfh.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://ysj.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxy.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://ljo.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://izo.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://alr.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zbr.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xkt.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rao.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yeu.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kzd.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vun.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://gqq.birdmap.top

Py:   now + timedelta(days=7)
来源：http://gwj.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vdr.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dnc.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://atl.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://rvr.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bwm.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://wrl.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://mkn.gzhubu.top

[J06] 计算两时间之差
来源：http://hnb.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://apf.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://gkg.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://epa.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qlx.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://csh.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://dwk.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://lgi.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://ysn.cqqwz.cn

[J07] 比较两个日期
来源：http://idn.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://rwq.52xcode.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vgl.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://jqz.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qjp.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://seh.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mfu.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://vfa.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ygd.guowangkeji.top

[J08] 提取年月日与星期
来源：http://hdf.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bhx.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uef.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xsv.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vnn.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://teh.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://atz.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wub.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://trr.hongshengwenyu.top

[J09] 时区处理
来源：http://wtc.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mhe.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hsx.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omq.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://klm.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nyu.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://izr.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tyf.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hes.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://cuu.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iml.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tur.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://olo.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hjh.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oad.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jew.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xxs.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lwz.pycfn.com

================================================================================
来源：http://akg.fzhhl.top

K. JSON 与序列化
来源：http://cff.jinqigufen.top

================================================================================
来源：http://jsj.vehdjk.com

[K01] 对象转 JSON 字符串
来源：http://mdr.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ujf.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uco.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://rmc.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://arh.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://khy.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://zns.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://fnx.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://euc.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://hlw.yfazqb.com

Py:   json.loads(s)
来源：http://egh.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wjf.yj20258888.top

JS:   JSON.parse(s)
来源：http://pew.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://dxg.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rpq.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://xlc.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://wfc.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://glc.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://neg.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xsv.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hlb.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kuu.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zfl.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://joy.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zqx.zhiwuduotai.top


<!-- 参考信息 -->