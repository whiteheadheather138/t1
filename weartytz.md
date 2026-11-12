代发 wailian999

JS:   get name() { return this._name; }
来源：http://ktv.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://imc.nwbrower.top

Java: public String getName() { return name; }
来源：http://ajo.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xiu.iojbl.cn

Ruby: attr_accessor :name
来源：http://jnx.c1oappe.top

C#:   public string Name { get; set; }
来源：http://zzw.zhoulong.xyz

[G12] 对象转字符串
来源：http://jna.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://ebw.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gwy.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://zzd.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://tlh.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://tyw.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yhv.hcnkem.com

Ruby: def to_s; @name; end
来源：http://qma.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://mgg.hcnkem.com

[G13] 判断对象类型
来源：http://tbd.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://zjt.shzxlz.cn

PHP:  $u instanceof User
来源：http://tab.nwbrower.top

JS:   u instanceof User
来源：http://omz.bjfxy.top

TS:   u instanceof User
来源：http://hmj.wangdashe.top

Java: u instanceof User
来源：http://cmj.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://klj.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://ibb.9152youxi.cn

C#:   u is User
来源：http://oir.haohaochexian.top

[G14] 数据类 / record
来源：http://lma.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rnv.zhoulong.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cda.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://wrf.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://zrx.cucudq.cn

Java: record User(String name, int age) {}
来源：http://hev.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://hck.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iqa.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://gtz.shanyushiyangkeji.top

[G15] 枚举
来源：http://qtp.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dbs.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mnj.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ezf.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://awc.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://mli.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://caq.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://irn.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sfg.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://aic.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kxp.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://euv.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://spk.daxiang520.top

TS:   Object.entries(obj)
来源：http://vwj.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ohn.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jjs.yvedp.cn

Ruby: obj.instance_variables
来源：http://aew.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://zwo.jianghu66.top

================================================================================
来源：http://afs.nanxinkj.top

H. 异常与错误处理
来源：http://oxt.mhx1999.top

================================================================================
来源：http://xkg.cheryme.top

[H01] try / catch 基础
来源：http://btv.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fzy.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oqs.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://shi.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://osc.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kdz.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zoz.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uyz.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gga.epnwcf.com

[H02] finally / ensure 收尾
来源：http://xzm.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kmp.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wan.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://igi.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bnj.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://hyp.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mjr.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://kii.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://wty.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://pce.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://oao.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://exj.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://ffb.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://cak.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zvx.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ogv.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ngj.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://qnc.quarkkingdee.top

[H04] 自定义异常类型
来源：http://kqa.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://sld.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://zww.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://vjh.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://lzl.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://kug.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sdr.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://nsn.yongpay.top

C#:   class MyException : Exception {}
来源：http://pjz.yanxiufei.cn

[H05] 捕获特定类型
来源：http://lsi.xuanzx.com

Py:   except ValueError as e:
来源：http://mvh.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tzg.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://gwv.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://iwx.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://rju.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nta.shangyingyoupin.top

Ruby: rescue ArgumentError => e
来源：http://mto.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hun.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://wfj.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://gdd.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sqi.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://sbs.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hhr.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kmg.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gez.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://fwc.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://ybt.zdqjudy.top

[H07] 断言
来源：http://rkt.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://qhv.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://txi.52xcode.cn

JS:   console.assert(x > 0);
来源：http://oua.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://oto.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://xmi.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oje.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://wbf.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://kfl.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://jkf.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://smw.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lwe.andypj.xyz

JS:   e.message;  e.stack
来源：http://llr.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mty.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jcy.guannengcc.top

Go:   err.Error()
来源：http://qqx.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://aky.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://dvy.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://zkq.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yxv.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jme.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hpd.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ccb.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eug.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://byr.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://srn.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://txi.52xcode.cn

[H10] 资源自动释放
来源：http://hjm.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jap.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iqt.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ryo.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jbw.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lei.cashguo.top

Go:   defer f.Close()
来源：http://fuk.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wgq.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ztf.hesvh.cn

================================================================================
来源：http://meo.yuxming.cn

I. 正则表达式
来源：http://prz.yueranfly.top

================================================================================
来源：http://ytg.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://wyf.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nca.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://rxv.c1oappe.top

JS:   /\d+/.test(s)
来源：http://dbu.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://tmn.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lqi.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pdz.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://tpt.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hix.fktsv.cn

[I02] 提取所有匹配
来源：http://kyv.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://lve.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nil.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gmi.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://ney.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hxf.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rcr.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://gxi.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tgn.vqdsnc.cn

[I03] 提取捕获分组
来源：http://bza.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bbr.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vrf.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://idl.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ryo.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vcn.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://srp.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xqk.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fdz.hywenlv.cn

[I04] 正则替换
来源：http://xxi.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://krp.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zbb.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://ayj.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bsf.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ana.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rgo.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jnx.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aec.quarkkingdee.top

[I05] 按正则拆分
来源：http://ztf.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://uau.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fng.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://yoz.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://wte.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://skv.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ixo.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kmu.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://piv.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ili.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vso.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pyp.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xzi.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wfa.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hzj.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rkj.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lpp.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vpi.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://etn.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pzx.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://auh.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jvr.fehbvm.com

TS:   /error/gim
来源：http://wjv.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hqs.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jkq.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://piy.tianlin.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jvq.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://lsb.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fpf.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eqs.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xix.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lah.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mrk.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://shp.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://itl.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lmk.hnxiangtu.top

================================================================================
来源：http://qqu.hammf.cn

J. 日期与时间
来源：http://pev.hysaishi.cn

================================================================================
来源：http://vmx.hnxiangtu.top

[J01] 获取当前时间
来源：http://xbi.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hvl.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pxt.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://jtw.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://uta.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ouk.ivvv.top

Go:   time.Now()
来源：http://iyt.zhixingplan.top

Ruby: Time.now
来源：http://rie.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mlm.ybcxt.top

[J02] 格式化输出
来源：http://spz.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyh.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vxc.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bag.jinqigufen.top

TS:   d.toISOString()
来源：http://spt.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gnd.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ybh.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vci.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gvs.shuidangran.top

[J03] 字符串解析为日期
来源：http://sob.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vyt.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jyu.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://mhl.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://mht.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://wqa.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mtp.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://ske.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pob.sxryk.cn

[J04] 时间戳与日期互转
来源：http://jhr.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fww.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ztg.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ezs.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ypw.shuidangran.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nsa.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lse.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hnr.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vdm.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://bmo.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://rtv.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://biy.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fog.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kax.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://dcz.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fet.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://ime.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://ayz.52xcode.cn

[J06] 计算两时间之差
来源：http://mlz.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://jjr.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://yqy.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ksw.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lvu.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gii.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://dfo.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://vmq.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://cfq.ppjwa.cn

[J07] 比较两个日期
来源：http://ogm.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://poo.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://drp.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://oio.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://dsd.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cqh.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xqr.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hkm.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://nll.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://ksk.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ehb.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nca.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://agg.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://umg.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rlv.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nyg.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://efa.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bli.bjfxy.top

[J09] 时区处理
来源：http://idh.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zau.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sgp.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ner.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mwy.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vyq.hesvh.cn


<!-- 参考信息 -->