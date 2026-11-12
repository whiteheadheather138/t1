代发 wailian999

JS:   get name() { return this._name; }
来源：http://mto.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://wjm.chenlongwang.top

Java: public String getName() { return name; }
来源：http://zko.jyoumei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dbh.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://lga.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://pzd.zhongyouzk.top

[G12] 对象转字符串
来源：http://otx.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://hhg.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mzz.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://qce.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://vgw.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://sjq.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://imf.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://ddb.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://kab.tarul.cn

[G13] 判断对象类型
来源：http://aig.tanke756.top

Py:   isinstance(u, User)
来源：http://jvr.cdnleiting.top

PHP:  $u instanceof User
来源：http://uor.sysykeji.top

JS:   u instanceof User
来源：http://csm.52xcode.cn

TS:   u instanceof User
来源：http://xxq.smart0.xyz

Java: u instanceof User
来源：http://unu.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://mak.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://wen.zhiwuduotai.top

C#:   u is User
来源：http://qel.ydzc1.top

[G14] 数据类 / record
来源：http://xdl.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://meu.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://bta.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://xhd.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://nyo.iojbl.cn

Java: record User(String name, int age) {}
来源：http://asn.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://pxe.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fwc.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://mpv.hongshengwenyu.top

[G15] 枚举
来源：http://oqa.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zzf.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://psr.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://goe.yvedp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yan.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://xvu.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jas.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://cux.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vto.yj20258.top

[G16] 对象转数组 / 字典
来源：http://ywr.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://owg.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://gyo.hammf.cn

JS:   Object.entries(obj)
来源：http://zbi.cqqwz.cn

TS:   Object.entries(obj)
来源：http://sds.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tcf.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ulw.shzxlz.cn

Ruby: obj.instance_variables
来源：http://jur.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://dqu.aizwys.cn

================================================================================
来源：http://hdn.nwbrower.top

H. 异常与错误处理
来源：http://tma.yj20258.top

================================================================================
来源：http://fvx.jianghu66.top

[H01] try / catch 基础
来源：http://zck.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rqv.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ksk.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jbz.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hte.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jgl.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jnc.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hdp.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://btw.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://ele.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://otg.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://sny.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://sfu.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://oxk.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://kwa.feifeiyinyue.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tiz.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sdr.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xwl.tanke756.top

[H03] 主动抛出异常
来源：http://yqk.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://zxp.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ukg.tanke756.top

JS:   throw new Error("错误信息");
来源：http://wjo.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://bdn.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://imf.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oip.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mqs.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://tiz.mhx1999.top

[H04] 自定义异常类型
来源：http://air.uphjek.com

Py:   class MyError(Exception): pass
来源：http://fjj.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hcu.zycfv.cn

JS:   class MyError extends Error {}
来源：http://rbr.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://syc.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://fak.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zlg.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://vrq.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://apn.zhixingplan.top

[H05] 捕获特定类型
来源：http://vxs.jqgfzy.top

Py:   except ValueError as e:
来源：http://eah.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ipc.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://qux.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://wcy.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://rhh.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bfz.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://gyn.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qgk.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://hdo.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://wtu.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://gft.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://yhk.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://ltq.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://knk.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tzt.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://pmz.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://ssq.chenlongwang.top

[H07] 断言
来源：http://ono.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://mom.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://pkq.zhiwuduotai.top

JS:   console.assert(x > 0);
来源：http://zgc.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://snu.yuanzhike.top

Java: assert x > 0 : "必须为正";
来源：http://ach.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lap.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wvf.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://dxe.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://bnk.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://vny.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gxy.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://vml.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uoq.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zhs.gzhubu.top

Go:   err.Error()
来源：http://mny.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://tnd.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://tuz.jinqigufen.top

[H09] 带错误码的异常
来源：http://ctd.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qbx.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cgd.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pck.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xsy.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uzb.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uxk.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nfd.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xvq.xylfe.cn

[H10] 资源自动释放
来源：http://uzu.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lql.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://erc.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qtf.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vab.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kbu.fzhhl.top

Go:   defer f.Close()
来源：http://baz.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://crl.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ezq.yj202588.top

================================================================================
来源：http://cgm.svipenyu.cn

I. 正则表达式
来源：http://kfy.xziqi.cn

================================================================================
来源：http://emd.gaohongyu789.top

[I01] 判断是否匹配
来源：http://iid.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hde.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://wda.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://dbp.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://lns.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zau.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fzw.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://qyb.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xne.birdmap.top

[I02] 提取所有匹配
来源：http://onr.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://wzj.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxx.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uvz.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://eri.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ikz.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qwo.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://fkj.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nzo.yvedp.cn

[I03] 提取捕获分组
来源：http://wpk.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yms.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vjt.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gud.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cfi.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rks.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ilo.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ezr.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xeo.feifeiyinyue.top

[I04] 正则替换
来源：http://pvf.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qsa.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ufw.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://udr.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://qdc.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://gxn.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oid.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ikz.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bld.fehbvm.com

[I05] 按正则拆分
来源：http://uiz.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eus.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ilx.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://qpq.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://xvp.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://zle.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gpj.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eqg.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wyb.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://grp.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rcm.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wnz.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gsx.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eoe.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://awh.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fmp.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xeo.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uig.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://hil.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zsh.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://auv.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rfm.cheryme.top

TS:   /error/gim
来源：http://qjf.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dvu.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zvh.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://vsy.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sei.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://zug.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vrk.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://leq.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfw.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zaj.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vng.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cdu.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jly.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kpu.tanke756.top

================================================================================
来源：http://lkl.pycfn.com

J. 日期与时间
来源：http://jjs.jiagoushi.top

================================================================================
来源：http://nbt.zhengqikj.top

[J01] 获取当前时间
来源：http://ric.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vxi.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pqg.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://kjj.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://kne.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zga.yongpay.top

Go:   time.Now()
来源：http://aql.tianlin.xyz

Ruby: Time.now
来源：http://rfz.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cut.tarul.cn

[J02] 格式化输出
来源：http://qfo.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxk.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://msm.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://viv.daxiang520.top

TS:   d.toISOString()
来源：http://hvs.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mgu.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lbv.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vyk.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vwa.nwbrower.top

[J03] 字符串解析为日期
来源：http://tjb.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wfp.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://scq.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://tbv.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://khu.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://zsb.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bra.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://cbu.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://afo.hnqzz.top

[J04] 时间戳与日期互转
来源：http://uoh.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dkr.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://who.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xcn.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fwp.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pob.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nma.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fmk.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://riy.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://qxh.cheryme.top

Py:   now + timedelta(days=7)
来源：http://eod.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://thp.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffa.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ith.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://kax.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xwl.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://ozb.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://bzv.0kj1m.cn

[J06] 计算两时间之差
来源：http://xih.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://hvu.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://yag.gzhubu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ovy.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://afp.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://oen.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://gks.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://jyn.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://qks.hongshengwenyu.top

[J07] 比较两个日期
来源：http://axd.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://vfi.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rrn.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://zqh.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://etm.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xjk.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tws.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://svs.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://flm.zdbjq.cn

[J08] 提取年月日与星期
来源：http://ffg.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bmd.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bce.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://leu.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cax.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vfh.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://teu.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wcm.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vee.tianlin.xyz

[J09] 时区处理
来源：http://bca.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://erb.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rdu.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ubs.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://drz.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cja.fengsongda.top


<!-- 参考信息 -->