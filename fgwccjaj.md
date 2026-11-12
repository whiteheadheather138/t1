代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xjk.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fjo.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://xsi.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vwv.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://hbd.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vnr.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://ohi.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://whb.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://lts.wangdashe.top

JS:   Object.entries(obj)
来源：http://bvf.hnqzz.top

TS:   Object.entries(obj)
来源：http://onr.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://msl.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jpt.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://kig.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://fau.yj202588.top

================================================================================
来源：http://kxd.ybcxt.top

H. 异常与错误处理
来源：http://ehn.hnqzz.top

================================================================================
来源：http://sss.xylfe.cn

[H01] try / catch 基础
来源：http://skp.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mal.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qbf.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yxi.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://niv.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oot.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jnn.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pjk.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xaz.yvedp.cn

[H02] finally / ensure 收尾
来源：http://xwa.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://ebk.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pjh.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rlr.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cee.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://ibr.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ltl.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cvi.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pqq.xziqi.cn

[H03] 主动抛出异常
来源：http://atj.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://vzx.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vru.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://mto.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://vpw.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nux.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kkk.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://apd.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jjn.quarkkingdee.top

[H04] 自定义异常类型
来源：http://szb.316326.xyz

Py:   class MyError(Exception): pass
来源：http://tor.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://hcp.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://tyx.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://ijh.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://cca.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tkl.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://glc.cucudq.cn

C#:   class MyException : Exception {}
来源：http://yqf.hnqzz.top

[H05] 捕获特定类型
来源：http://gfu.tanke756.top

Py:   except ValueError as e:
来源：http://udm.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yuh.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://zye.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://udf.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://zrm.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mmu.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://eap.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jho.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://uyq.yvedp.cn

Py:   value = d.get("k") or default
来源：http://jny.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://hqe.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://oaq.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://nfs.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fwy.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bnl.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://bzg.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://mkf.shuidangran.top

[H07] 断言
来源：http://pom.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://mra.hesvh.cn

PHP:  assert($x > 0);
来源：http://iuc.fzhhl.top

JS:   console.assert(x > 0);
来源：http://qls.andypj.xyz

TS:   console.assert(x > 0);
来源：http://fxk.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://rxp.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ozo.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://trh.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://zct.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://anl.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://dbt.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lvi.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://wim.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rxm.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oxf.9152youxi.cn

Go:   err.Error()
来源：http://vot.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://smz.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://dok.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://gmt.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ztj.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bvt.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qzr.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://del.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zqe.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yzu.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://rqh.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://hga.dashuyun.cn

[H10] 资源自动释放
来源：http://fui.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aks.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cgc.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nag.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fns.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vtv.jinqigufen.top

Go:   defer f.Close()
来源：http://rrc.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mtp.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fny.tarul.cn

================================================================================
来源：http://mtn.zhiwuduotai.top

I. 正则表达式
来源：http://clb.ctjpmb.com

================================================================================
来源：http://scw.fehbvm.com

[I01] 判断是否匹配
来源：http://wzx.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dob.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://oue.fehbvm.com

JS:   /\d+/.test(s)
来源：http://bay.xylfe.cn

TS:   /\d+/.test(s)
来源：http://jva.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uxi.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wbk.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://koi.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bhy.havefunace.top

[I02] 提取所有匹配
来源：http://sij.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://znj.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gzi.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fsz.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://jpz.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jge.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cal.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://cut.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://afc.ydzc1.top

[I03] 提取捕获分组
来源：http://ntb.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zua.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://afk.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hnk.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fny.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zvu.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cfx.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bph.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rsp.jlsjyb.cn

[I04] 正则替换
来源：http://owz.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jrs.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wly.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wqc.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://kbq.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nxy.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jxs.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kyz.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://imf.daria6918.cn

[I05] 按正则拆分
来源：http://xco.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qjt.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xfd.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://awf.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://mqp.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://zfh.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pdk.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://rmi.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gdm.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://flh.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yiy.yuanzhike.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pws.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qna.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://grp.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://laa.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kle.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tcw.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pgl.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://tdm.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://exx.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uhl.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://znx.ivvv.top

TS:   /error/gim
来源：http://nro.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://acr.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oba.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://nka.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wmq.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://yom.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bkr.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kho.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ryo.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mxd.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qkt.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ogu.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bkh.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fcm.svipenyu.cn

================================================================================
来源：http://nxz.hnqzz.top

J. 日期与时间
来源：http://zqd.zhongyouzk.top

================================================================================
来源：http://tka.hcnkem.com

[J01] 获取当前时间
来源：http://vnc.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rxb.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fup.nwbrower.top

JS:   new Date();  Date.now()
来源：http://zhv.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://fug.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tig.ybcxt.top

Go:   time.Now()
来源：http://tbq.zycfv.cn

Ruby: Time.now
来源：http://smn.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yfw.jinqigufen.top

[J02] 格式化输出
来源：http://rkp.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://llm.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jeh.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aal.dashuyun.cn

TS:   d.toISOString()
来源：http://die.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xvm.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bic.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jlf.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mrj.cqqwz.cn

[J03] 字符串解析为日期
来源：http://hos.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://frq.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yjo.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://kvq.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://ctx.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iit.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ahp.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://wby.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mbz.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://jct.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ywt.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sbu.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://exi.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lti.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pzo.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bgj.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://shk.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jra.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://gdt.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://fsj.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cga.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iwd.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cmy.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://bpy.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lfe.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://dnb.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pwj.jyoumei.cn

[J06] 计算两时间之差
来源：http://lhd.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://vlq.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://ysh.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://whm.jiagoushi.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dfm.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://qyl.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://cur.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://pop.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://pws.hfpthk.cn

[J07] 比较两个日期
来源：http://ijn.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://tll.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ilc.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://juf.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iug.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vvg.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hly.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xyq.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://fwk.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://ece.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ime.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bkf.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://awx.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gks.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://scu.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yls.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fza.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jyc.cheryme.top

[J09] 时区处理
来源：http://pny.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://emc.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nue.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hlq.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ofw.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rac.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mrl.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ctv.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hmu.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://hkz.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cfc.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bgh.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uou.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uca.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bsg.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zfr.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ylt.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qep.kuanghao11.cn

================================================================================
来源：http://ynz.gzhubu.top

K. JSON 与序列化
来源：http://lka.9152youxi.cn

================================================================================
来源：http://pen.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://afh.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mtd.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kih.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://xiq.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://rpa.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vuw.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://cth.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://gnm.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://hur.yfazqb.com

[K02] JSON 字符串转对象
来源：http://gny.ctjpmb.com

Py:   json.loads(s)
来源：http://dyv.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ven.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://spd.hesvh.cn

TS:   JSON.parse(s)
来源：http://fhj.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjd.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://sal.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://rel.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://web.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://pjm.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hlq.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rdc.cashguo.top


<!-- 参考信息 -->