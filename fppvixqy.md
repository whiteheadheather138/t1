代发 wailian999

[G14] 数据类 / record
来源：http://buj.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lsu.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://zqx.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ndn.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://nsm.sweek.top

Java: record User(String name, int age) {}
来源：http://aso.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://cix.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kiw.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://aoy.ybcxt.top

[G15] 枚举
来源：http://fvl.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://whe.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ysy.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yqv.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://awa.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://ggn.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gme.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://jpa.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tso.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://fgt.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fet.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://ken.fehbvm.com

JS:   Object.entries(obj)
来源：http://wgk.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://uvj.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jer.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lay.nanxinkj.top

Ruby: obj.instance_variables
来源：http://pok.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://jgr.chenjidiqi.icu

================================================================================
来源：http://rbc.vehdjk.com

H. 异常与错误处理
来源：http://opn.hongshengwenyu.top

================================================================================
来源：http://rsr.snrcjt.cn

[H01] try / catch 基础
来源：http://qfo.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://whk.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bai.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jrs.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xqu.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dah.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://smx.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://exl.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rlq.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://kap.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vhj.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iyd.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jfj.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ydl.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zee.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ilc.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oks.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jfg.iojbl.cn

[H03] 主动抛出异常
来源：http://uwh.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://zer.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cgo.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://eqm.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://tvp.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tsc.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rjf.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cre.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://tyv.nanxinkj.top

[H04] 自定义异常类型
来源：http://zmm.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://kua.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://gzr.nwbrower.top

JS:   class MyError extends Error {}
来源：http://nqa.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://wvh.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://ace.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gvn.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://wrs.pycfn.com

C#:   class MyException : Exception {}
来源：http://wbl.hesvh.cn

[H05] 捕获特定类型
来源：http://eau.zhengqikj.top

Py:   except ValueError as e:
来源：http://zng.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pfh.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://ang.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://ape.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://tte.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rhs.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://chc.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nxu.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://ysx.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://lzf.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tad.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sdt.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jxz.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://otp.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://slc.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://tcv.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://vey.ywan-chungtsiang.top

[H07] 断言
来源：http://uxt.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://lxa.cheryme.top

PHP:  assert($x > 0);
来源：http://buw.yueranfly.top

JS:   console.assert(x > 0);
来源：http://lgo.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://roq.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://yeb.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cnl.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eyk.tarul.cn

C#:   Debug.Assert(x > 0);
来源：http://rda.cqqwz.cn

[H08] 获取错误信息与堆栈
来源：http://xvw.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://vfs.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mbr.mhx1999.top

JS:   e.message;  e.stack
来源：http://bdy.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://awu.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://dds.ydjk.org.cn

Go:   err.Error()
来源：http://loz.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://vxu.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://uyl.shuidangran.top

[H09] 带错误码的异常
来源：http://fyx.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gre.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://egy.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tqv.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://liu.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xxn.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://viv.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fvs.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qqu.gogol.net.cn

[H10] 资源自动释放
来源：http://ztl.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jrg.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xgw.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ffl.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hbv.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dyc.tarul.cn

Go:   defer f.Close()
来源：http://yjt.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hhl.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yqw.tarul.cn

================================================================================
来源：http://pft.birdmap.top

I. 正则表达式
来源：http://equ.zhiwuduotai.top

================================================================================
来源：http://fms.wangdashe.top

[I01] 判断是否匹配
来源：http://odc.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wws.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://aph.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://epo.xylfe.cn

TS:   /\d+/.test(s)
来源：http://aze.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bkl.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ndc.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://axn.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ddd.ydjk.org.cn

[I02] 提取所有匹配
来源：http://ylz.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://oxe.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wjk.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://buo.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://bjf.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qsg.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://skn.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://arn.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://evb.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://qhy.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yqc.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://knk.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ahj.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qju.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aod.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://goj.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xwq.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vwr.zhixingplan.top

[I04] 正则替换
来源：http://umu.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lmt.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ims.redwolf501.top

JS:   s.replace(/\d+/g, "#")
来源：http://vgj.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://bhl.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://pyt.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://vjh.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://aiw.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ogh.svipenyu.cn

[I05] 按正则拆分
来源：http://bph.kuanghao11.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bbl.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://imd.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://gsa.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://bbs.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://nfx.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qtw.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://edr.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fbn.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tkd.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ddh.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hll.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dhb.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fra.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zfv.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kcn.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://szo.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://svn.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://dgd.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://try.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kbq.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kud.xziqi.cn

TS:   /error/gim
来源：http://cdg.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fab.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://njb.tarul.cn

Ruby: s.scan(/error/i)
来源：http://xmg.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wto.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://elo.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aba.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hbm.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hso.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qar.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tit.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pcv.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wks.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mee.daxiang520.top

================================================================================
来源：http://ddu.ywan-chungtsiang.top

J. 日期与时间
来源：http://yfs.yfazqb.com

================================================================================
来源：http://ztp.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://fgx.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gkj.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rlp.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://qon.yj20258.top

TS:   new Date();  Date.now()
来源：http://pmj.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vpn.tianlin.xyz

Go:   time.Now()
来源：http://umf.ydzc1.top

Ruby: Time.now
来源：http://vqt.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mzr.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://kui.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzs.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wnt.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fht.yonumen.top

TS:   d.toISOString()
来源：http://yxi.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fif.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ula.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gam.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cjr.xuanzx.com

[J03] 字符串解析为日期
来源：http://ixw.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aba.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zvc.birdmap.top

JS:   new Date("2024-01-02")
来源：http://khy.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://rjg.sufxvd.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nar.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://des.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://ymv.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vat.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://sho.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://scq.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ynn.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://edn.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://iqp.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hga.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ruy.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gcn.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bvr.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://jzd.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://uab.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://isf.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fnt.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yen.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://ucw.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bxy.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://tii.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fkw.0kj1m.cn

[J06] 计算两时间之差
来源：http://ptb.yj202588.top

Py:   (end - start).total_seconds()
来源：http://bew.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://gti.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tpl.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fdt.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://mbc.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://elt.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://exe.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://ews.tianlin.xyz

[J07] 比较两个日期
来源：http://fvr.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://mej.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://roi.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://qnj.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ioi.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nyc.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dbr.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://grd.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://uar.cheryme.top

[J08] 提取年月日与星期
来源：http://cyk.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://heu.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yod.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vkj.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://red.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dyp.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rai.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://opv.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://omz.xziqi.cn

[J09] 时区处理
来源：http://ofw.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lwp.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ntc.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zjo.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tlu.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vct.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://enp.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lty.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xju.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://xbi.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pfc.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfo.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ekj.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sti.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zxk.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jfw.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fmh.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zwz.yj20258.top

================================================================================
来源：http://gjn.hnqzz.top

K. JSON 与序列化
来源：http://yfi.xuanzx.com

================================================================================
来源：http://cjm.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://zoe.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hqx.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ayc.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://xni.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://vdo.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ryv.fzhhl.top

Go:   json.Marshal(obj)
来源：http://dsm.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xmk.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qhb.yvedp.cn


<!-- 参考信息 -->