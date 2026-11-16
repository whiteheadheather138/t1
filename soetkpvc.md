代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://thu.yj20258.top

JS:   toString() { return this.name; }
来源：http://knm.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://nvp.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://wih.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://mcs.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://uks.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://uml.jinqigufen.top

[G13] 判断对象类型
来源：http://ehk.jianghu66.top

Py:   isinstance(u, User)
来源：http://fyq.yvedp.cn

PHP:  $u instanceof User
来源：http://spi.zhijiandao.cn

JS:   u instanceof User
来源：http://drq.bbcook.cn

TS:   u instanceof User
来源：http://ihq.fktsv.cn

Java: u instanceof User
来源：http://jye.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nry.daxiang520.top

Ruby: u.is_a?(User)
来源：http://vnn.zhoulong.xyz

C#:   u is User
来源：http://wwu.bbcook.cn

[G14] 数据类 / record
来源：http://tfm.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zww.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://nfw.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://djo.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://sis.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://ecs.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://uwu.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zmd.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://qox.yanxiufei.cn

[G15] 枚举
来源：http://rkz.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kou.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://thu.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qcn.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iuf.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://hvd.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mtb.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://ydk.zhixingplan.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xcb.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://pmf.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://itx.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://zcs.ehwqpu.com

JS:   Object.entries(obj)
来源：http://htg.xuanzx.com

TS:   Object.entries(obj)
来源：http://trv.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xhp.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://afk.guowangkeji.top

Ruby: obj.instance_variables
来源：http://ljm.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://jfs.ydjk.org.cn

================================================================================
来源：http://uwx.daxiang520.top

H. 异常与错误处理
来源：http://mro.wangshuangyany.cn

================================================================================
来源：http://isv.iojbl.cn

[H01] try / catch 基础
来源：http://vgc.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lqx.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rnv.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://emw.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bxp.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vkg.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lfx.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vod.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dzs.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://oft.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wqh.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://krz.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hup.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jct.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hkx.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://owf.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ioe.hongshengwenyu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uro.hysaishi.cn

[H03] 主动抛出异常
来源：http://lpi.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://fjy.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rkp.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://snw.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://wco.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://csz.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kwt.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tmb.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dge.0kj1m.cn

[H04] 自定义异常类型
来源：http://hov.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://uhk.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://hjx.52xcode.cn

JS:   class MyError extends Error {}
来源：http://igm.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://now.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://pea.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://slr.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://tpp.sweek.top

C#:   class MyException : Exception {}
来源：http://mdu.vehdjk.com

[H05] 捕获特定类型
来源：http://doq.aibaodan.cn

Py:   except ValueError as e:
来源：http://vff.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tjg.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://ugj.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://vno.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://ejt.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ciu.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://pnb.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cdu.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://zmf.xziqi.cn

Py:   value = d.get("k") or default
来源：http://ypm.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://blx.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://row.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://tzz.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tzy.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kds.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://tgd.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://zuh.fengsongda.top

[H07] 断言
来源：http://hct.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://bwv.tianlin.xyz

PHP:  assert($x > 0);
来源：http://xoh.sysykeji.top

JS:   console.assert(x > 0);
来源：http://irq.tian-w.cn

TS:   console.assert(x > 0);
来源：http://ukl.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://kpk.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eie.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://vnw.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://txy.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://knh.zdqjudy.top

Py:   str(e);  traceback.format_exc()
来源：http://ftc.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sdb.fzhhl.top

JS:   e.message;  e.stack
来源：http://frz.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dgm.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kfc.zhijiandao.cn

Go:   err.Error()
来源：http://erf.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://sxb.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://ret.yanxiufei.cn

[H09] 带错误码的异常
来源：http://bhz.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lxq.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xvo.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kgr.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ghu.shzxlz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kwy.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dgf.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://ocd.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sar.jyoumei.cn

[H10] 资源自动释放
来源：http://ruk.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://lbf.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://keg.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aof.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wdl.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dbl.jqgufenzy.top

Go:   defer f.Close()
来源：http://lre.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qrx.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zyw.xziqi.cn

================================================================================
来源：http://blt.shuidangran.top

I. 正则表达式
来源：http://vru.havefunace.top

================================================================================
来源：http://rwe.zhongyouzk.top

[I01] 判断是否匹配
来源：http://ohb.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dxv.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zzs.mhx1999.top

JS:   /\d+/.test(s)
来源：http://vnn.52xcode.cn

TS:   /\d+/.test(s)
来源：http://eqo.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pxz.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wrj.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://odt.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bzb.jinqigufen.top

[I02] 提取所有匹配
来源：http://ilz.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://ytq.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jqv.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jmg.pycfn.com

TS:   s.match(/\d+/g)
来源：http://dgh.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dco.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jrd.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://rum.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mgs.ybcxt.top

[I03] 提取捕获分组
来源：http://mkh.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqa.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://imh.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hkd.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fnz.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://drs.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hes.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yau.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://phr.316326.xyz

[I04] 正则替换
来源：http://ijr.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://yho.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pwc.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://krj.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jdf.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://rxr.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vli.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xni.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iaz.aizwys.cn

[I05] 按正则拆分
来源：http://lew.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rxt.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qrr.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://eft.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://oex.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://vbf.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ilf.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://qpi.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jis.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qcb.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fia.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cae.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ful.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gxw.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bom.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jss.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cru.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dwh.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://zsc.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gyx.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yjl.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://seu.9152youxi.cn

TS:   /error/gim
来源：http://mwd.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lfw.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tmg.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://wmu.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dsa.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://ane.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vzg.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tim.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hun.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wpz.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://toy.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zth.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ted.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cta.jinqigfzy.top

================================================================================
来源：http://xzy.jinghuilouyu.cn

J. 日期与时间
来源：http://vqj.hysaishi.cn

================================================================================
来源：http://soe.yongpay.top

[J01] 获取当前时间
来源：http://esh.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://jep.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://arp.yj20258.top

JS:   new Date();  Date.now()
来源：http://olk.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://nme.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pnz.yj20258888.top

Go:   time.Now()
来源：http://uwk.0kj1m.cn

Ruby: Time.now
来源：http://rcw.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cvz.cucudq.cn

[J02] 格式化输出
来源：http://haj.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dnu.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dwb.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kte.haohaochexian.top

TS:   d.toISOString()
来源：http://byl.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ldr.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rvf.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ykg.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ynm.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://jxj.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xne.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vfj.yj20258.top

JS:   new Date("2024-01-02")
来源：http://hbw.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://txd.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ccz.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pqn.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://hth.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bqv.hongshengwenyu.top

[J04] 时间戳与日期互转
来源：http://jyr.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mtf.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fpp.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://utd.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lit.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wzh.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rhg.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gll.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ulw.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://gqi.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://mgt.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xjy.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ytt.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vwl.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://wkt.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://csc.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://qud.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://usx.zhoulong.xyz

[J06] 计算两时间之差
来源：http://sll.meibo888.top

Py:   (end - start).total_seconds()
来源：http://jub.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://hsb.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://keb.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aju.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://tcy.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://tcn.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://xxh.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://iqa.tian-w.cn

[J07] 比较两个日期
来源：http://vvw.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://vfq.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vdr.uphjek.com

JS:   d1.getTime() < d2.getTime()
来源：http://xhw.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jvn.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pqj.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ojm.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://clo.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://evw.mhx1999.top

[J08] 提取年月日与星期
来源：http://kmg.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cud.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dez.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aii.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oks.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jwu.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://enf.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sua.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dpc.yangfankeji.com

[J09] 时区处理
来源：http://iyk.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zov.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bel.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yaa.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ljm.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kwk.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qod.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://bvr.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uph.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://evm.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://afu.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uti.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://goa.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uge.snrcjt.cn


<!-- 参考信息 -->