代发 wailian999

C#:   public / protected / private / internal
来源：http://iov.redwolf501.top

[G11] getter / setter
来源：http://hfg.xziqi.cn

Py:   @property 与 @x.setter
来源：http://pfa.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://djq.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://xlk.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://jak.hysaishi.cn

Java: public String getName() { return name; }
来源：http://puo.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ahg.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://rsd.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://ben.xziqi.cn

[G12] 对象转字符串
来源：http://sgh.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://ccq.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hmd.smart0.xyz

JS:   toString() { return this.name; }
来源：http://dxr.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://nvt.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://fik.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://goo.yj20258.top

Ruby: def to_s; @name; end
来源：http://jwm.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://ndg.havefunace.top

[G13] 判断对象类型
来源：http://ztv.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://bto.havefunace.top

PHP:  $u instanceof User
来源：http://ssz.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://lys.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://mwd.gogol.net.cn

Java: u instanceof User
来源：http://efa.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nqa.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://kvr.jianghu66.top

C#:   u is User
来源：http://cak.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://bbf.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qtv.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://gcz.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vmq.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://pth.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://etv.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://vvn.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cuw.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://vfa.shuidangran.top

[G15] 枚举
来源：http://tnn.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bte.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ics.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pip.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dtq.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://adt.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lrw.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://efo.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wge.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://gxf.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dlc.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://drb.yj20258888.top

JS:   Object.entries(obj)
来源：http://oya.sufxvd.cn

TS:   Object.entries(obj)
来源：http://ygy.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mli.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://azn.gogol.net.cn

Ruby: obj.instance_variables
来源：http://hyy.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://smz.xylfe.cn

================================================================================
来源：http://ncy.pycfn.com

H. 异常与错误处理
来源：http://ylz.ywan-chungtsiang.top

================================================================================
来源：http://vza.sufxvd.cn

[H01] try / catch 基础
来源：http://mbq.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wqg.shanyushiyangtech.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pnq.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uue.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hsf.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dxv.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://asu.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://onu.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sfe.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://tbg.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tey.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ehu.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qao.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yqh.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://mde.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xof.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://svj.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aut.redwolf501.top

[H03] 主动抛出异常
来源：http://jvp.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://iqn.jinyuanbaomall.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hzv.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://jgw.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://ona.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dmf.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bdy.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yya.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zpq.quarkkingdee.top

[H04] 自定义异常类型
来源：http://bts.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://cwg.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yyd.aizwys.cn

JS:   class MyError extends Error {}
来源：http://afe.zycfv.cn

TS:   class MyError extends Error {}
来源：http://xos.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://yxa.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rcl.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://enq.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://mfk.iojbl.cn

[H05] 捕获特定类型
来源：http://lck.sysykeji.top

Py:   except ValueError as e:
来源：http://ppl.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://svx.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://mzu.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://hyz.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://pff.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lrc.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://zxt.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ivf.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://rsj.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://wjb.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://edk.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://mrc.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://jvb.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nxt.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dxw.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://vlc.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://ndw.nwbrower.top

[H07] 断言
来源：http://wnc.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://mdc.chenzaomai.com

PHP:  assert($x > 0);
来源：http://grl.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://czp.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://jio.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://jne.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cqr.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://int.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://yyq.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://kzs.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://lfw.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lab.aizwys.cn

JS:   e.message;  e.stack
来源：http://lgz.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://rxq.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zot.nwbrower.top

Go:   err.Error()
来源：http://oea.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://mrp.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://sfa.zdbjq.cn

[H09] 带错误码的异常
来源：http://vnk.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vvv.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gkl.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hwt.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://anp.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vds.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fau.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://whm.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ntl.yangfankeji.com

[H10] 资源自动释放
来源：http://lrh.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://frm.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bzu.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sng.xuetiantiany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://adw.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lul.chenlongwang.top

Go:   defer f.Close()
来源：http://oql.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zyt.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://prf.pycfn.com

================================================================================
来源：http://qvj.yangfankeji.com

I. 正则表达式
来源：http://yoy.c1oappe.top

================================================================================
来源：http://zap.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://uka.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sgq.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://lhl.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://nwc.sweek.top

TS:   /\d+/.test(s)
来源：http://khx.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yaa.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tmo.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://dkp.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jmb.yangfankeji.com

[I02] 提取所有匹配
来源：http://spg.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://izs.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qrl.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hkx.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://ofx.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://szl.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ted.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://sbf.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ezj.gogol.net.cn

[I03] 提取捕获分组
来源：http://wdu.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tbo.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qhh.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yys.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nup.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ktp.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://meh.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ykg.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://miw.zhaomingkeji.xyz

[I04] 正则替换
来源：http://oyc.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cid.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fsk.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://mnd.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://bdt.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://asj.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://spb.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://efi.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ktw.gogol.net.cn

[I05] 按正则拆分
来源：http://dfk.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tzq.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sqt.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://sjc.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://mvv.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://mbj.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wds.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://woq.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mbr.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jed.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iuf.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xgv.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lfn.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://puq.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vxx.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nfk.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qfh.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hat.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://fpm.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://njm.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ruo.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cuj.ivvv.top

TS:   /error/gim
来源：http://bmm.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ini.wangshuangyany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://naq.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://lzr.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://stx.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://oec.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ygg.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lyi.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ruh.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://coe.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rbe.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qay.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qnm.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hjp.feifeiyinyue.top

================================================================================
来源：http://jeh.xinyue.icu

J. 日期与时间
来源：http://nbz.pycfn.com

================================================================================
来源：http://kzb.chenjidiqi.icu

[J01] 获取当前时间
来源：http://amc.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rju.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rez.tarul.cn

JS:   new Date();  Date.now()
来源：http://qqg.guannengcc.top

TS:   new Date();  Date.now()
来源：http://lqv.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://iik.yvedp.cn

Go:   time.Now()
来源：http://spu.yueranfly.top

Ruby: Time.now
来源：http://evt.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://two.havefunace.top

[J02] 格式化输出
来源：http://tog.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bea.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xxf.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://apg.cqqwz.cn

TS:   d.toISOString()
来源：http://zkn.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://krk.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cpp.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mpz.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iqy.hnqzz.top

[J03] 字符串解析为日期
来源：http://hfj.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yme.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://smv.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://lle.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://xvp.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ocw.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://obv.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://oki.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wms.xuanzx.com

[J04] 时间戳与日期互转
来源：http://svg.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jhf.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lxt.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jlm.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://zyk.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sir.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qqd.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uob.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zck.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://rjo.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://moc.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lkj.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fsk.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ioj.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://juu.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wio.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://tmp.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://bge.yuanzhike.top

[J06] 计算两时间之差
来源：http://yaw.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://qrj.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://deu.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ztb.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qvp.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jqy.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://las.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://nis.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://kcs.tarul.cn

[J07] 比较两个日期
来源：http://mha.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://xft.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vim.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://upc.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://upl.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://btd.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ewg.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lxm.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://uxu.bbcook.cn

[J08] 提取年月日与星期
来源：http://aul.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rvy.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tkj.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yab.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oqx.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fwn.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pbk.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iza.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://usm.sxryk.cn

[J09] 时区处理
来源：http://wic.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ivw.daria6918.cn


<!-- 参考信息 -->