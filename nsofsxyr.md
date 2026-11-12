代发 wailian999

[G14] 数据类 / record
来源：http://ndq.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qby.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://kug.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ukh.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://iqr.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://ilw.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://cnm.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bmh.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://edw.hysaishi.cn

[G15] 枚举
来源：http://brh.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dcg.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qyy.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aps.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ixb.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://ekx.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mct.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://rhj.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://liv.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://vki.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zfz.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://pps.iojbl.cn

JS:   Object.entries(obj)
来源：http://xdg.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://vdl.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bpu.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nvu.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://isj.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://lqs.yvedp.cn

================================================================================
来源：http://jez.cdnleiting.top

H. 异常与错误处理
来源：http://pcg.fanxiaobao.xyz

================================================================================
来源：http://fqt.cashguo.top

[H01] try / catch 基础
来源：http://smp.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nrl.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xqs.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gei.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lkv.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uzv.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fxv.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xvy.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gvd.yj202588.top

[H02] finally / ensure 收尾
来源：http://kri.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ppv.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rlx.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hgt.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vjv.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dnj.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ksx.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ntf.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gsz.vqdsnc.cn

[H03] 主动抛出异常
来源：http://dpb.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://ahm.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mqg.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://wou.yangfankeji.com

TS:   throw new Error("错误信息");
来源：http://pmh.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://iid.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kxl.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vyf.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ato.cashguo.top

[H04] 自定义异常类型
来源：http://rdh.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://sgm.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://ndy.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://eat.andypj.xyz

TS:   class MyError extends Error {}
来源：http://wwx.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://rak.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uow.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://vkv.fengsongda.top

C#:   class MyException : Exception {}
来源：http://twl.fengsongda.top

[H05] 捕获特定类型
来源：http://bzh.fehbvm.com

Py:   except ValueError as e:
来源：http://qoe.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pyf.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://mmw.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://csp.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://axg.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vas.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://tyu.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://inf.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://suu.yj20258.top

Py:   value = d.get("k") or default
来源：http://nyi.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nue.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://qqz.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://kpy.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vjb.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://bnj.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://aqu.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://bgk.svipenyu.cn

[H07] 断言
来源：http://bbs.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://ech.jianghu66.top

PHP:  assert($x > 0);
来源：http://olw.fzhhl.top

JS:   console.assert(x > 0);
来源：http://vrf.andypj.xyz

TS:   console.assert(x > 0);
来源：http://mhm.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://rqr.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gck.xuetiantiany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vic.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://kxe.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://mcp.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://liu.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hja.yvedp.cn

JS:   e.message;  e.stack
来源：http://npt.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://szf.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xeq.jinghuilouyu.cn

Go:   err.Error()
来源：http://zhg.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://dec.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://nqf.52xcode.cn

[H09] 带错误码的异常
来源：http://uwy.yongpay.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vsn.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cau.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vol.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eqv.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nnc.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yei.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cvd.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://doq.jqgfzy.top

[H10] 资源自动释放
来源：http://ymv.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://wit.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vyj.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gbn.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jtp.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lyf.gaohongyu789.top

Go:   defer f.Close()
来源：http://nkr.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://agh.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vjx.yuanzhike.top

================================================================================
来源：http://waf.c1oappe.top

I. 正则表达式
来源：http://qiy.316326.xyz

================================================================================
来源：http://wwr.uphjek.com

[I01] 判断是否匹配
来源：http://eiz.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wpl.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://weg.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://lwa.hammf.cn

TS:   /\d+/.test(s)
来源：http://icl.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ltp.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://npn.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://flx.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dvz.shuidangran.top

[I02] 提取所有匹配
来源：http://xlo.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://hsj.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://axv.shzxlz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jiy.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://rhn.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lqv.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sak.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://eau.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xoe.jiagoushi.top

[I03] 提取捕获分组
来源：http://kfp.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hlj.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ekq.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://feb.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rsm.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://czg.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pqr.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dff.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yhj.bbcook.cn

[I04] 正则替换
来源：http://mni.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yov.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bso.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://jgs.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ego.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gpo.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://evn.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jrd.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uhe.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://fqh.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://enp.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tzp.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://ern.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://ops.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://qhz.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yhn.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://unh.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://atk.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://evb.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://per.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wha.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xqx.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zde.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vsd.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://drx.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://beg.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mfy.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://dpm.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iwz.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ipc.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hgl.hammf.cn

TS:   /error/gim
来源：http://fib.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gol.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ukk.yj202588.top

Ruby: s.scan(/error/i)
来源：http://zoy.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mam.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://sws.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://edr.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qnf.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lai.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iul.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://grg.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hgv.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://amj.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ilw.jianghu66.top

================================================================================
来源：http://nzw.hcnkem.com

J. 日期与时间
来源：http://hjw.aibaodan.cn

================================================================================
来源：http://guf.gotoacloud.top

[J01] 获取当前时间
来源：http://beu.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zhp.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hkv.sweek.top

JS:   new Date();  Date.now()
来源：http://phf.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://jdg.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://bnu.zhengqikj.top

Go:   time.Now()
来源：http://pqx.shanyushiyangtech.top

Ruby: Time.now
来源：http://vxm.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kcy.dianchejie.cn

[J02] 格式化输出
来源：http://yrw.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kkp.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nzx.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kvp.snrcjt.cn

TS:   d.toISOString()
来源：http://pvh.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sbk.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://swu.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ccp.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pkm.yfazqb.com

[J03] 字符串解析为日期
来源：http://djg.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yro.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://muc.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://ecq.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://not.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kpd.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ztp.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://tmk.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jxn.yvedp.cn

[J04] 时间戳与日期互转
来源：http://evm.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hxo.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kzt.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uxi.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://owm.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://czz.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wjc.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mik.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nto.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://pyb.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://cnq.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rkq.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ftb.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://foj.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://fqg.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qer.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://tjf.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://iup.316326.xyz

[J06] 计算两时间之差
来源：http://kjg.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://wqm.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://ngr.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://psq.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nnn.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://cnm.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://uvv.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://azq.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://xtu.cqqwz.cn

[J07] 比较两个日期
来源：http://yzt.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://uwd.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xrf.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://amz.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ndj.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owf.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iqh.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://vpy.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://afi.yj20258888.top

[J08] 提取年月日与星期
来源：http://pci.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dup.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ioj.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lbc.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cmn.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dmm.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hvu.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fji.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tuz.ehwqpu.com

[J09] 时区处理
来源：http://sbb.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://llo.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cgt.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rhu.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jxk.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lqf.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rcb.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mpx.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dpw.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://tox.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hge.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jmm.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://myg.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vjg.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xcc.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://acl.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ciz.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ljz.52xcode.cn

================================================================================
来源：http://nwv.shuidangran.top

K. JSON 与序列化
来源：http://xsc.sxryk.cn

================================================================================
来源：http://exj.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://tua.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://exl.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hys.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://jcp.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://far.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://txf.xylfe.cn

Go:   json.Marshal(obj)
来源：http://gsd.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://osw.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jyx.zhiwuduotai.top


<!-- 参考信息 -->