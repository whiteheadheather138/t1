代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://fqx.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://qcj.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://hyt.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pup.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://glc.hnqzz.top

[G15] 枚举
来源：http://lqx.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kdu.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rrn.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://byt.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zfh.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://qwl.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pnn.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://irl.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://otz.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://jls.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ulw.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://via.gogol.net.cn

JS:   Object.entries(obj)
来源：http://jet.fktsv.cn

TS:   Object.entries(obj)
来源：http://fok.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://alv.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xwc.52xcode.cn

Ruby: obj.instance_variables
来源：http://txn.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://jut.yj20258888.top

================================================================================
来源：http://lpz.sjlbkw.cn

H. 异常与错误处理
来源：http://rzg.cdnleiting.top

================================================================================
来源：http://ezb.birdmap.top

[H01] try / catch 基础
来源：http://jsh.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eod.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ufl.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://psf.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jnr.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://col.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lrp.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hou.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dwc.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://wdv.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://mxz.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vrl.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wwb.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qzl.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hxw.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jfj.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ozp.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rqn.zycfv.cn

[H03] 主动抛出异常
来源：http://yby.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://ewu.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aok.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://frt.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://jnk.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fpu.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://anu.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pfq.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://bdx.zhijiandao.cn

[H04] 自定义异常类型
来源：http://ghj.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://phq.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ovr.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://hgu.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://kzu.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://mcd.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eqm.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://mjl.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://fsr.zhixingplan.top

[H05] 捕获特定类型
来源：http://daj.zdbjq.cn

Py:   except ValueError as e:
来源：http://gnu.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://icj.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://ygg.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://okz.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://oqm.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hqe.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://nfv.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://niq.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://dia.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://hiu.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://ubp.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mlo.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://bht.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qbg.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mae.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://cjh.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://mzl.cdnleiting.top

[H07] 断言
来源：http://ywf.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://nsh.tianlin.xyz

PHP:  assert($x > 0);
来源：http://tfe.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://jfh.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://mxo.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://mgq.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mcx.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://qeu.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://wcv.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://fix.fktsv.cn

Py:   str(e);  traceback.format_exc()
来源：http://alj.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cqa.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://ycb.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gel.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tde.jqgufenzy.top

Go:   err.Error()
来源：http://fyd.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://rww.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://fzg.zhoulong.xyz

[H09] 带错误码的异常
来源：http://cjf.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://znq.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hpd.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sbg.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wes.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fcc.aizwys.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qjw.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iaw.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://one.9152youxi.cn

[H10] 资源自动释放
来源：http://cib.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://gcy.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jsw.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cnn.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ivl.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dsj.aibaodan.cn

Go:   defer f.Close()
来源：http://grv.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qiq.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rpl.yueranfly.top

================================================================================
来源：http://bgy.jiagoushi.top

I. 正则表达式
来源：http://ofz.ybcxt.top

================================================================================
来源：http://vmc.vehdjk.com

[I01] 判断是否匹配
来源：http://dxs.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://erh.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://uts.gzhubu.top

JS:   /\d+/.test(s)
来源：http://xaz.daria6918.cn

TS:   /\d+/.test(s)
来源：http://une.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yuf.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fcn.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://jiy.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jrl.gzhubu.top

[I02] 提取所有匹配
来源：http://asj.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://sco.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vbh.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yhv.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://azs.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fxg.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yxv.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://ddq.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kxu.yj20258.top

[I03] 提取捕获分组
来源：http://odt.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lhn.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://agd.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jic.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uti.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tud.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fzx.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ugi.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bks.bbcook.cn

[I04] 正则替换
来源：http://njz.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hfu.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kbs.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://smc.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gqw.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://xnm.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pwx.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ggr.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hxi.xuetiantiany.cn

[I05] 按正则拆分
来源：http://xdh.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pak.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hyo.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://nks.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://wea.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://moh.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sjb.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://htu.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uec.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vjl.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dfl.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nnm.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qff.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cks.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vql.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fgy.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://smr.bbcook.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zzg.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://ovb.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nhp.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qlz.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ygt.shanyushiyangtech.top

TS:   /error/gim
来源：http://lvq.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hxv.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sww.cashguo.top

Ruby: s.scan(/error/i)
来源：http://yer.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://avj.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://utu.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tkp.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ztc.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ono.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezg.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fhx.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zme.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lwj.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://svi.sxryk.cn

================================================================================
来源：http://ndn.dashuyun.cn

J. 日期与时间
来源：http://gkn.fehbvm.com

================================================================================
来源：http://ekn.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://tvz.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mkl.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ire.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://ros.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://cth.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kne.havefunace.top

Go:   time.Now()
来源：http://mlk.jinyuanbaomall.cn

Ruby: Time.now
来源：http://ozl.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pej.yongpay.top

[J02] 格式化输出
来源：http://glf.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tnh.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://myf.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bly.hongshengwenyu.top

TS:   d.toISOString()
来源：http://czl.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tdg.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhw.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nav.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bjq.ivvv.top

[J03] 字符串解析为日期
来源：http://glj.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rkf.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://geh.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://sep.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://oip.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dqo.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lqe.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://qrb.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mnu.havefunace.top

[J04] 时间戳与日期互转
来源：http://ntb.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zgt.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oso.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ggk.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fsp.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ppo.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rsd.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://otr.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://inr.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://dvi.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://fld.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rvz.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lui.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xov.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://bxw.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nyb.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://ktm.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://ysk.redwolf501.top

[J06] 计算两时间之差
来源：http://lrc.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://kpu.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://qvs.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tou.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aob.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://rpg.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://nyw.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://euz.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://zoy.quarkkingdee.top

[J07] 比较两个日期
来源：http://hqw.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://apk.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hdt.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://xbe.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gwz.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gei.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kbu.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rjw.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://wkm.guowangkeji.top

[J08] 提取年月日与星期
来源：http://ita.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgv.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://khe.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ijh.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mrq.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kfn.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ogt.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mzo.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bjg.dianchejie.cn

[J09] 时区处理
来源：http://otw.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://abh.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dto.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pin.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcr.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kbj.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hpg.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tnw.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zxm.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://nls.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ren.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://byw.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nrw.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iuf.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mii.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tkt.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rku.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pjk.kuanghao11.cn

================================================================================
来源：http://spm.sufxvd.cn

K. JSON 与序列化
来源：http://ysx.xuetiantiany.cn

================================================================================
来源：http://pxc.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://sbi.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://btt.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://foc.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://kyr.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://nkg.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sfc.gzhubu.top

Go:   json.Marshal(obj)
来源：http://kwj.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://ktp.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tyd.52xcode.cn

[K02] JSON 字符串转对象
来源：http://utp.yanxiufei.cn

Py:   json.loads(s)
来源：http://chh.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qra.shzxlz.cn

JS:   JSON.parse(s)
来源：http://zbh.dashuyun.cn


<!-- 参考信息 -->