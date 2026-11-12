代发 wailian999

TS:   public / protected / private
来源：http://jao.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://pso.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wda.yfazqb.com

Ruby: public / protected / private
来源：http://bpp.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://uaq.jyoumei.cn

[G11] getter / setter
来源：http://lxm.nwbrower.top

Py:   @property 与 @x.setter
来源：http://oal.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sgn.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://otw.haohaochexian.top

TS:   get name(): string { return this._name; }
来源：http://zei.yuxming.cn

Java: public String getName() { return name; }
来源：http://tbh.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hwy.xinyue.icu

Ruby: attr_accessor :name
来源：http://mzj.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://hyp.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://vxn.yongpay.top

Py:   def __str__(self): return self.name
来源：http://bai.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ojw.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://lru.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://zjn.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://eco.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://raq.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://oyd.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://vab.sxryk.cn

[G13] 判断对象类型
来源：http://srm.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://mdu.ctjpmb.com

PHP:  $u instanceof User
来源：http://eie.bjfxy.top

JS:   u instanceof User
来源：http://mrp.shzxlz.cn

TS:   u instanceof User
来源：http://uwy.zdbjq.cn

Java: u instanceof User
来源：http://ktk.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://erf.yuxming.cn

Ruby: u.is_a?(User)
来源：http://acp.dianchejie.cn

C#:   u is User
来源：http://mdm.feifeiyinyue.top

[G14] 数据类 / record
来源：http://fdx.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vnv.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://czr.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ajk.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://xgd.yuxming.cn

Java: record User(String name, int age) {}
来源：http://mie.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://gep.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ulb.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://xqc.yangfankeji.com

[G15] 枚举
来源：http://dye.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ipf.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hrs.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ihf.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ngp.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://sgb.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xcm.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://pab.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jsp.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://pnx.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://btj.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://xid.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://zds.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://ixe.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pdv.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://yky.yuanzhike.top

Ruby: obj.instance_variables
来源：http://sjw.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://qqj.yonumen.top

================================================================================
来源：http://lih.zhongyouzk.top

H. 异常与错误处理
来源：http://wci.ydzc1.top

================================================================================
来源：http://ctd.yvedp.cn

[H01] try / catch 基础
来源：http://qzb.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gca.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://isc.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bpo.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ylk.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qht.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lyp.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bex.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hyr.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://qoq.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://luy.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xxr.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hct.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tcc.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://svd.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wbk.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vbt.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ulv.haohaochexian.top

[H03] 主动抛出异常
来源：http://eti.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://wlp.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ilf.tanke756.top

JS:   throw new Error("错误信息");
来源：http://qbt.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://njh.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mmc.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vci.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iqq.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://dcb.fehbvm.com

[H04] 自定义异常类型
来源：http://ori.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://zmy.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://sea.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://srp.yj202588.top

TS:   class MyError extends Error {}
来源：http://rmn.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://wvl.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wkl.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://wdv.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://srz.sjlbkw.cn

[H05] 捕获特定类型
来源：http://sqz.iojbl.cn

Py:   except ValueError as e:
来源：http://dtp.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kxa.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://srm.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://dul.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://tjq.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fwa.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://rdv.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oql.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://vna.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://oes.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://tel.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xke.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://wrx.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://thh.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vzu.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://ghv.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://tyh.yj202588.top

[H07] 断言
来源：http://kha.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://qhn.hysaishi.cn

PHP:  assert($x > 0);
来源：http://fjf.tanke756.top

JS:   console.assert(x > 0);
来源：http://qrh.hcnkem.com

TS:   console.assert(x > 0);
来源：http://izv.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ump.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://owo.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://vtm.zhixingplan.top

C#:   Debug.Assert(x > 0);
来源：http://yvq.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://oyx.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://cpt.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oao.dashuyun.cn

JS:   e.message;  e.stack
来源：http://qyh.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zrr.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vvr.hfpthk.cn

Go:   err.Error()
来源：http://dru.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://gmr.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://kqv.epnwcf.com

[H09] 带错误码的异常
来源：http://sil.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pdj.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pqy.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xpv.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rzt.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kaj.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://brc.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://epu.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://rwr.nwbrower.top

[H10] 资源自动释放
来源：http://pxp.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rgc.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ift.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rhe.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yky.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gqm.yanxiufei.cn

Go:   defer f.Close()
来源：http://xww.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ptw.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xpm.jinyuanbaomall.cn

================================================================================
来源：http://jro.dashuyun.cn

I. 正则表达式
来源：http://yli.hfpthk.cn

================================================================================
来源：http://jbx.tarul.cn

[I01] 判断是否匹配
来源：http://hsw.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rsi.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://afb.gzhubu.top

JS:   /\d+/.test(s)
来源：http://vwe.cashguo.top

TS:   /\d+/.test(s)
来源：http://dzw.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cab.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://krm.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://fou.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lnl.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://hon.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://vxj.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fgu.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://afq.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://bft.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://akr.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://esr.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://swb.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kgj.jianghu66.top

[I03] 提取捕获分组
来源：http://gpd.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uhn.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lzs.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jnr.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vyj.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zkp.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hzi.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uhb.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iwn.zhengqikj.top

[I04] 正则替换
来源：http://ypg.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mfz.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://udk.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://cho.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://bdk.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://aon.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://bzh.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oke.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zmv.birdmap.top

[I05] 按正则拆分
来源：http://rai.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://kwo.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uyc.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://jgm.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://hjm.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://otw.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eag.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://jtt.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wek.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lvs.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kor.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xpp.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://avn.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uww.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qwf.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bxs.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nft.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vjz.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://oqc.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yct.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://miy.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fvk.redwolf501.top

TS:   /error/gim
来源：http://hgp.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pjt.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://luj.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://kmt.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ucj.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://peq.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mws.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://exs.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xck.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qwo.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gur.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zfx.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sqi.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://npn.jinyuanbaomall.cn

================================================================================
来源：http://qwd.mhx1999.top

J. 日期与时间
来源：http://ijf.nanxuanxn.top

================================================================================
来源：http://myg.wangdashe.top

[J01] 获取当前时间
来源：http://qcj.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://clw.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mpi.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://myu.epnwcf.com

TS:   new Date();  Date.now()
来源：http://yop.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vjm.iojbl.cn

Go:   time.Now()
来源：http://jqq.ctjpmb.com

Ruby: Time.now
来源：http://eft.chenlongwang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xsk.jiagoushi.top

[J02] 格式化输出
来源：http://ljj.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kgc.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hmn.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qlq.mhx1999.top

TS:   d.toISOString()
来源：http://yuk.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ull.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jfk.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mck.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jeo.zhixingplan.top

[J03] 字符串解析为日期
来源：http://exc.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jjf.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://otu.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://syg.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://irx.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://ofa.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dlt.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://isj.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tib.fzhhl.top

[J04] 时间戳与日期互转
来源：http://hwe.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uer.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dlm.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yfm.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lin.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nkn.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bsb.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kwv.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xsl.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://eyv.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://mjf.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fwa.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yfp.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://byt.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://wpz.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hxf.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://mux.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://edm.fehbvm.com

[J06] 计算两时间之差
来源：http://zgn.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://loz.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://qca.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rkg.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wvz.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://gmj.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://dzq.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://nvm.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://eei.zdqjudy.top

[J07] 比较两个日期
来源：http://jef.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://cxx.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yxx.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jar.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://oer.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nux.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wdp.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://ofx.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://jxi.ehwqpu.com

[J08] 提取年月日与星期
来源：http://hhy.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xnr.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ezd.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ndi.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tgc.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qqn.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nnc.tanke756.top


<!-- 参考信息 -->