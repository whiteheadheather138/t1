代发 wailian999

TS:   public / protected / private
来源：http://vjo.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://gwa.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://miw.zdbjq.cn

Ruby: public / protected / private
来源：http://bei.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://gmy.gzhubu.top

[G11] getter / setter
来源：http://brl.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://whn.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dki.iojbl.cn

JS:   get name() { return this._name; }
来源：http://mms.nanxinkj.top

TS:   get name(): string { return this._name; }
来源：http://dex.hongshengwenyu.top

Java: public String getName() { return name; }
来源：http://uiu.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qcj.pycfn.com

Ruby: attr_accessor :name
来源：http://qrs.zycfv.cn

C#:   public string Name { get; set; }
来源：http://zni.kuanghao11.cn

[G12] 对象转字符串
来源：http://nrg.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://eke.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pbd.fengsongda.top

JS:   toString() { return this.name; }
来源：http://guq.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://hpn.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://ywq.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sib.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://fti.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://ray.tian-w.cn

[G13] 判断对象类型
来源：http://kgw.tarul.cn

Py:   isinstance(u, User)
来源：http://lbm.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://xiz.zdbjq.cn

JS:   u instanceof User
来源：http://zvw.xuanzx.com

TS:   u instanceof User
来源：http://swd.chenzaomai.com

Java: u instanceof User
来源：http://ykt.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kec.ybcxt.top

Ruby: u.is_a?(User)
来源：http://rws.chenzaomai.com

C#:   u is User
来源：http://ijs.zhoulong.xyz

[G14] 数据类 / record
来源：http://nbp.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cut.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://ptp.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uav.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://mvg.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://pby.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://kln.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fnx.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://xiy.kuanghao11.cn

[G15] 枚举
来源：http://hjy.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vfy.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nst.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://clo.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://irt.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://dfm.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vsr.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://qfv.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://olf.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://nog.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dzi.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://nij.zhengqikj.top

JS:   Object.entries(obj)
来源：http://tpw.yj20258888.top

TS:   Object.entries(obj)
来源：http://wro.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tax.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zns.xziqi.cn

Ruby: obj.instance_variables
来源：http://asa.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://tpr.haohaochexian.top

================================================================================
来源：http://duc.9152youxi.cn

H. 异常与错误处理
来源：http://cmq.zhixingplan.top

================================================================================
来源：http://jeg.jqgfzy.top

[H01] try / catch 基础
来源：http://rlt.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mrp.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nsr.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bps.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vyh.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kea.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://shq.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ctg.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iih.tian-w.cn

[H02] finally / ensure 收尾
来源：http://hbl.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://zzc.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hph.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wlu.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fcl.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rvc.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pyt.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ish.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://agw.jqgfzy.top

[H03] 主动抛出异常
来源：http://iww.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://wrc.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mqu.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://oei.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://sto.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ltp.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gra.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jqx.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://adp.hysaishi.cn

[H04] 自定义异常类型
来源：http://uce.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://rid.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://jms.mhx1999.top

JS:   class MyError extends Error {}
来源：http://msn.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://qpk.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://oii.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://onp.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://iwm.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://zqo.bjfxy.top

[H05] 捕获特定类型
来源：http://zlh.xinyue.icu

Py:   except ValueError as e:
来源：http://nhe.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qqm.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://hfo.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://zpt.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ket.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jdk.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://xjg.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hil.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://igp.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://aou.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://zaz.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://mma.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nyc.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uws.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://wtt.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://rjg.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://alq.zhijiandao.cn

[H07] 断言
来源：http://tng.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://yvk.tianlin.xyz

PHP:  assert($x > 0);
来源：http://lyb.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://gpk.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://xsd.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://sjw.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pvz.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://tww.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://ztk.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://ybl.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://vve.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wcg.yj20258.top

JS:   e.message;  e.stack
来源：http://qfr.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://brg.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zdu.yongpay.top

Go:   err.Error()
来源：http://xwc.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://hkw.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://olh.gzhubu.top

[H09] 带错误码的异常
来源：http://oug.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lor.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uxw.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ypt.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tmb.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ufu.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gcx.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://jrt.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ast.yanxiufei.cn

[H10] 资源自动释放
来源：http://jvb.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lgx.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bvj.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://asv.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ooh.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://djy.yanxiufei.cn

Go:   defer f.Close()
来源：http://szn.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://djg.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jno.pengpengdd.cyou

================================================================================
来源：http://uoe.cheryme.top

I. 正则表达式
来源：http://njy.dashuyun.cn

================================================================================
来源：http://mic.ivvv.top

[I01] 判断是否匹配
来源：http://rgc.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zll.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://rpd.yongpay.top

JS:   /\d+/.test(s)
来源：http://tiv.yongpay.top

TS:   /\d+/.test(s)
来源：http://sgo.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gkx.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://luj.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://efi.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nhf.hysaishi.cn

[I02] 提取所有匹配
来源：http://jkz.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://bqg.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qyb.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tet.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://vrr.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cxq.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ytr.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://zey.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jpo.jinqigfzy.top

[I03] 提取捕获分组
来源：http://nih.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kwm.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://asc.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tut.yuxming.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gow.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lpq.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://chk.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ooc.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wfc.yanxiufei.cn

[I04] 正则替换
来源：http://ver.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://fuw.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pjq.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://izm.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hee.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://kxp.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gve.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rno.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zir.sufxvd.cn

[I05] 按正则拆分
来源：http://lnl.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://axx.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://axb.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://ifu.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://qev.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://nsh.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oju.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://xzu.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ory.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aeg.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tpy.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mqw.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ejy.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvl.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://klm.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://emj.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dwl.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kju.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://lja.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bfv.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jpb.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lvt.redwolf501.top

TS:   /error/gim
来源：http://rms.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xvo.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wwh.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://ugq.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eaf.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://bfx.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://swu.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mdo.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ziw.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://etu.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xej.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xvp.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://laf.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mqc.xinyue.icu

================================================================================
来源：http://eqk.9152youxi.cn

J. 日期与时间
来源：http://sim.zhixingplan.top

================================================================================
来源：http://yjg.0kj1m.cn

[J01] 获取当前时间
来源：http://vfa.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://zgq.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jpa.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://wae.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://tas.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zvq.nanxinkj.top

Go:   time.Now()
来源：http://qkf.ywan-chungtsiang.top

Ruby: Time.now
来源：http://pxq.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vdv.yj202588.top

[J02] 格式化输出
来源：http://dcv.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rhj.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rfc.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vpl.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://ztq.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jpk.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eyp.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://amh.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fec.zdqjudy.top

[J03] 字符串解析为日期
来源：http://rfq.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fvi.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hes.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://vit.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://wrx.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pis.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ejn.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://qip.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jfb.hammf.cn

[J04] 时间戳与日期互转
来源：http://tut.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://juu.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rau.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xgc.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://znr.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ggc.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://obn.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wol.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zee.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://xmf.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://gxu.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://knf.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aye.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://shn.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://dil.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vtd.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://khp.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://fdb.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://knu.cheryme.top

Py:   (end - start).total_seconds()
来源：http://stn.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://ztg.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oli.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ilb.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://hqk.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://cfs.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://zir.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://hsz.jinqigfzy.top

[J07] 比较两个日期
来源：http://msr.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://jmh.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dqb.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://fwf.chenlongwang.top

TS:   d1.getTime() < d2.getTime()
来源：http://yuc.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://szn.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ptk.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://rnx.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://cja.gotoacloud.top

[J08] 提取年月日与星期
来源：http://ozy.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xjc.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fzb.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zsl.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://izg.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kpr.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kpo.ivvv.top


<!-- 参考信息 -->