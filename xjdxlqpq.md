代发 wailian999

JS:   get name() { return this._name; }
来源：http://puu.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://lhf.aibaodan.cn

Java: public String getName() { return name; }
来源：http://chi.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mzm.jqgfzy.top

Ruby: attr_accessor :name
来源：http://bff.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://avw.zhengqikj.top

[G12] 对象转字符串
来源：http://fql.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://yhk.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://eku.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://kcs.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://rhr.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://unl.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://otr.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://xyy.yj202588.top

C#:   public override string ToString() => Name;
来源：http://omk.nanxuanxn.top

[G13] 判断对象类型
来源：http://hiz.0kj1m.cn

Py:   isinstance(u, User)
来源：http://ehw.xziqi.cn

PHP:  $u instanceof User
来源：http://avx.0kj1m.cn

JS:   u instanceof User
来源：http://bkg.jianghu66.top

TS:   u instanceof User
来源：http://njb.jiagoushi.top

Java: u instanceof User
来源：http://xwv.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://uky.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://mwk.havefunace.top

C#:   u is User
来源：http://ryv.dianchejie.cn

[G14] 数据类 / record
来源：http://wof.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bke.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://mpd.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nlu.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://qho.mhx1999.top

Java: record User(String name, int age) {}
来源：http://gad.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://cee.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lgw.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://mpj.xingfuxueyuan.xyz

[G15] 枚举
来源：http://gwb.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wrf.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uvm.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ibn.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kmy.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://pow.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fyp.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://afo.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oac.meibo888.top

[G16] 对象转数组 / 字典
来源：http://otx.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vtm.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://mrn.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://cdk.gzhubu.top

TS:   Object.entries(obj)
来源：http://aqd.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rkg.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vun.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://nmd.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://nui.zdqjudy.top

================================================================================
来源：http://ugo.svipenyu.cn

H. 异常与错误处理
来源：http://fzk.fehbvm.com

================================================================================
来源：http://etn.jyoumei.cn

[H01] try / catch 基础
来源：http://wzj.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lya.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwg.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xio.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zeb.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kwe.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nva.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uqi.mhx1999.top

[H02] finally / ensure 收尾
来源：http://jmu.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kkl.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jbg.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fxp.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ebw.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://nzr.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tot.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vtg.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fja.epnwcf.com

[H03] 主动抛出异常
来源：http://mku.hfpthk.cn

Py:   raise ValueError("错误信息")
来源：http://qnl.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ian.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://bbu.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://wmn.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://czd.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vxo.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zpr.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://gkk.52xcode.cn

[H04] 自定义异常类型
来源：http://nmf.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://cxx.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eqv.shzxlz.cn

JS:   class MyError extends Error {}
来源：http://phq.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://ewr.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://bpo.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jft.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://wra.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://tja.havefunace.top

[H05] 捕获特定类型
来源：http://gmo.hywenlv.cn

Py:   except ValueError as e:
来源：http://raa.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://map.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://wil.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://vot.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://mho.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wpz.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://cpg.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xvo.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://hzz.fengsongda.top

Py:   value = d.get("k") or default
来源：http://bxy.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://irc.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://juv.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://bem.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dpz.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jwj.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://wgq.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://bpd.fehbvm.com

[H07] 断言
来源：http://qcs.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://bni.guannengcc.top

PHP:  assert($x > 0);
来源：http://kur.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://qav.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://jgi.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://bvf.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oag.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://qzm.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://fwd.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://voz.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://gmi.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pgc.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://rgk.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ayl.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://sca.daria6918.cn

Go:   err.Error()
来源：http://fks.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://mvm.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://pro.jyoumei.cn

[H09] 带错误码的异常
来源：http://uuf.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rfl.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ejk.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zuc.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eel.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zkp.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://psh.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ous.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nsy.cqqwz.cn

[H10] 资源自动释放
来源：http://xsi.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kxv.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tzm.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yqe.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iei.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://okk.wangshuangyany.cn

Go:   defer f.Close()
来源：http://fgm.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pyw.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://alq.316326.xyz

================================================================================
来源：http://eun.aizwys.cn

I. 正则表达式
来源：http://cao.jianghu66.top

================================================================================
来源：http://upw.ydjk.org.cn

[I01] 判断是否匹配
来源：http://ckm.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jir.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://rpk.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://dfp.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://hrw.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ugw.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yau.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://cft.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://toi.gogol.net.cn

[I02] 提取所有匹配
来源：http://vwt.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://rsm.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qbg.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tiu.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://uvq.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aif.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lqh.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://pnh.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rve.xziqi.cn

[I03] 提取捕获分组
来源：http://lun.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://glw.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kzg.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cic.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ptz.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lzq.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qmp.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mtk.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xvb.hesvh.cn

[I04] 正则替换
来源：http://gpw.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rsf.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fsz.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://xag.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://okm.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://fga.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zlc.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ivk.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kwn.chenlongwang.top

[I05] 按正则拆分
来源：http://cme.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tnq.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mpf.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://dpe.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://gtn.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://buq.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tck.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hdl.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ovy.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qmp.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pfc.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nrr.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ife.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ytt.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ayl.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rvd.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sas.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://inz.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://ydj.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kel.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://frw.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kbt.gzhubu.top

TS:   /error/gim
来源：http://rxr.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ypd.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ilr.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://ifn.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tik.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://muw.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lcw.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kzr.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jwm.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qdd.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://qbk.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dpv.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://znn.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yvj.zhixingplan.top

================================================================================
来源：http://eiq.tanke756.top

J. 日期与时间
来源：http://msg.jinqigfzy.top

================================================================================
来源：http://duu.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://kit.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sod.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lpf.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://uun.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://afg.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wkv.tian-w.cn

Go:   time.Now()
来源：http://vfk.zhiwuduotai.top

Ruby: Time.now
来源：http://afr.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dtu.vehdjk.com

[J02] 格式化输出
来源：http://byi.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qoy.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lib.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://awe.guowangkeji.top

TS:   d.toISOString()
来源：http://ayt.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pxv.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fdw.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fxy.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jcg.bjfxy.top

[J03] 字符串解析为日期
来源：http://avi.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://liy.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://weo.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://gre.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://mjz.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zjz.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://grw.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://ame.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jgy.redwolf501.top

[J04] 时间戳与日期互转
来源：http://hei.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pyt.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qed.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://atv.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ojo.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aui.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mbc.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bip.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ccl.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://tki.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://oel.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://klg.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://crj.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmx.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://sjj.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ott.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://zho.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://icj.xziqi.cn

[J06] 计算两时间之差
来源：http://cpg.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://yor.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://tlx.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bsv.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fre.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://emq.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://kya.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://sov.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://yfd.bjfxy.top

[J07] 比较两个日期
来源：http://czh.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://fkg.andypj.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eep.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://ywz.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://wdt.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mka.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qyi.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ykp.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://cgn.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://qpn.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://olb.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pwo.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rpx.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://awq.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ihh.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vzf.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mfs.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rlk.daxiang520.top

[J09] 时区处理
来源：http://vub.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ikc.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xrf.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uum.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hjw.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iug.fzhhl.top


<!-- 参考信息 -->