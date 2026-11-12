代发 wailian999

readonly PI=3.14
来源：http://fsf.zhoulong.xyz

[R04] 位置参数
来源：http://hhp.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mxz.yonumen.top

[R05] 参数默认值
来源：http://hgq.jinghuilouyu.cn

name="${1:-default}"
来源：http://nld.daxiang520.top

[R06] 判断命令是否存在
来源：http://sim.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ddp.sysykeji.top

[R07] if 判断文件
来源：http://zrq.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zvw.chenjidiqi.icu

[R08] 数值比较
来源：http://osq.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gqx.zhoulong.xyz

[R09] 字符串比较
来源：http://eoc.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://efg.xylfe.cn

[R10] 正则匹配
来源：http://ggg.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://knv.chenzaomai.com

[R11] case 多分支
来源：http://lmz.jqgfzy.top

case "$1" in
来源：http://byq.hongshengwenyu.top

start) echo "启动" ;;
来源：http://nks.wangdashe.top

stop)  echo "停止" ;;
来源：http://wwt.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://cbs.jianghu66.top

esac
来源：http://zhw.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://slf.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://xzn.smart0.xyz

[R13] for 计数循环
来源：http://vsx.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://wbj.sjlbkw.cn

[R14] C 风格 for
来源：http://sey.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gvg.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://ssq.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hzk.fengsongda.top

[R16] until 等待条件
来源：http://cxv.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gst.52xcode.cn

[R17] 数组定义与取值
来源：http://fyo.jinyuanbaomall.cn

arr=(a b c); echo "${arr[0]}"
来源：http://acx.quarkkingdee.top

[R18] 遍历数组
来源：http://aac.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ldn.bbcook.cn

[R19] 数组长度
来源：http://pin.meibo888.top

echo "${#arr[@]}"
来源：http://dro.daxiang520.top

[R20] 关联数组（字典）
来源：http://vft.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zrf.andypj.xyz

[R21] 字符串长度
来源：http://lnc.zhongyouzk.top

echo "${#s}"
来源：http://wyq.yangfankeji.com

[R22] 截取子串
来源：http://vee.havefunace.top

echo "${s:0:5}"
来源：http://riu.yangfankeji.com

[R23] 字符串替换
来源：http://cuw.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qpi.yvedp.cn

[R24] 大小写转换
来源：http://atd.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://pfw.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://gcn.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mwb.ehwqpu.com

[R26] 命令替换
来源：http://ibt.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://etu.0kj1m.cn

[R27] 算术展开
来源：http://rxi.wangdashe.top

echo $((1 + 2 * 3))
来源：http://ics.fktsv.cn

[R28] 浮点运算
来源：http://ghl.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://lbz.chenlongwang.top

[R29] 定义函数
来源：http://ckl.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://erk.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://wvn.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://oiw.zdqjudy.top

[R31] 局部变量
来源：http://nsr.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://pfu.cashguo.top

[R32] 参数个数校验
来源：http://pvv.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mml.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://pdn.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nsh.tanke756.top

[R34] 退出时清理
来源：http://khy.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://gfr.316326.xyz

[R35] 后台执行并等待
来源：http://pkp.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fyt.tianlin.xyz

[R36] 并发执行多个任务
来源：http://muf.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vpv.gotoacloud.top

[R37] 把输出赋给变量
来源：http://rly.xinyue.icu

files=$(ls -1)
来源：http://jzr.vqdsnc.cn

[R38] 管道串联
来源：http://qzk.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://ypg.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://eyp.jinqigufen.top

cmd > out.log 2>&1
来源：http://tsu.jinqigufen.top

[R40] 追加写日志
来源：http://lgd.quarkkingdee.top

echo "log" >> out.log
来源：http://zdf.hfpthk.cn

[R41] 丢弃输出
来源：http://ata.yj202588.top

cmd >/dev/null 2>&1
来源：http://fcn.gzhubu.top

[R42] 输入重定向
来源：http://rkk.sjlbkw.cn

wc -l < a.txt
来源：http://kly.bbcook.cn

[R43] 按名字查找文件
来源：http://qph.yonumen.top

find . -name "*.log" -type f
来源：http://hqb.hesvh.cn

[R44] 按修改时间查找
来源：http://mfl.hnxiangtu.top

find . -mtime -7 -type f
来源：http://zny.shanyushiyangkeji.top

[R45] 批量删除
来源：http://jfk.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://fyi.redwolf501.top

[R46] 递归替换文件内容
来源：http://xiq.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cgr.aibaodan.cn

[R47] sed 单行替换
来源：http://mjq.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://trs.sxryk.cn

[R48] awk 取指定列
来源：http://mwr.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://gvg.andypj.xyz

[R49] awk 带条件
来源：http://urf.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jkp.jinqigufen.top

[R50] awk 求和
来源：http://gji.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ebf.hnqzz.top

[R51] 排序去重取前几
来源：http://twu.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wgu.hongshengwenyu.top

[R52] 统计行数
来源：http://rvt.pengpengdd.cyou

wc -l a.txt
来源：http://iro.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://vza.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gta.ctjpmb.com

[R54] 比较两个文件
来源：http://adk.cucudq.cn

diff a.txt b.txt
来源：http://khy.jlsjyb.cn

[R55] 压缩与解压
来源：http://rfk.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hbi.sxryk.cn

[R56] 远程拷贝
来源：http://zpa.nanxuanxn.top

scp file user@host:/path/
来源：http://nto.cdnleiting.top

[R57] 远程执行命令
来源：http://llk.sufxvd.cn

ssh user@host 'uptime'
来源：http://whe.gotoacloud.top

[R58] 下载文件
来源：http://sip.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ame.ppjwa.cn

[R59] 发 POST JSON
来源：http://rnr.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ful.bbcook.cn

[R60] 只看 HTTP 状态码
来源：http://qvp.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qun.sysykeji.top

[R61] 磁盘占用
来源：http://qrn.xuetiantiany.cn

df -h;  du -sh *
来源：http://tzr.yuxming.cn

[R62] 找最占空间的文件
来源：http://xij.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://wsa.birdmap.top

[R63] 内存与进程
来源：http://eit.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://lfn.jyoumei.cn

[R64] 结束进程
来源：http://xtd.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://dma.dianchejie.cn

[R65] 查看端口占用
来源：http://drd.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cot.nanxinkj.top

[R66] 定时任务
来源：http://fqn.hysaishi.cn

crontab -e;  crontab -l
来源：http://jcy.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://orl.cheryme.top

openssl rand -hex 16
来源：http://vft.zdqjudy.top

[R68] 计算文件校验值
来源：http://ebs.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://pkm.hammf.cn

[R69] 生成随机密码
来源：http://awy.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://zcf.havefunace.top

[R70] 时间戳与互转
来源：http://acw.yonumen.top

date +%s;  date -d @1700000000
来源：http://grl.hysaishi.cn

[R71] 日期格式化
来源：http://stb.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ney.tian-w.cn

[R72] 等待端口就绪
来源：http://yvb.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ipp.zdbjq.cn

[R73] 分割大日志
来源：http://gkv.epnwcf.com

split -l 1000 big.log part_
来源：http://uzo.jlsjyb.cn

[R74] 批量重命名
来源：http://lxq.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cyr.yanxiufei.cn

[R75] 导出环境变量
来源：http://rnc.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://cqf.zycfv.cn

[R76] 使用临时文件
来源：http://zol.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ols.hesvh.cn

[R77] 读取用户输入
来源：http://fpg.zycfv.cn

read -rp "请输入: " ans
来源：http://ffw.vehdjk.com

[R78] 交互式菜单
来源：http://hzw.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nac.0kj1m.cn

[R79] 解析命令行选项
来源：http://xbp.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ymm.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://kdw.guowangkeji.top

time ./run.sh
来源：http://zrr.hnxiangtu.top

================================================================================
来源：http://sqc.zdqjudy.top

S. C / C++ 专题
来源：http://gyo.cucudq.cn

================================================================================
来源：http://imx.hfpthk.cn

[S01] C：Hello World
来源：http://vvc.fanxiaobao.xyz

#include <stdio.h>
来源：http://eyn.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://ysr.smart0.xyz

[S02] C：变量与格式化输出
来源：http://uib.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://hcs.iojbl.cn

[S03] C：读入整数
来源：http://wri.hywenlv.cn

int x; scanf("%d", &x);
来源：http://ekf.tanke756.top

[S04] C：字符串复制
来源：http://bdr.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://tzs.gogol.net.cn

[S05] C：字符串长度
来源：http://frz.zhijiandao.cn

strlen(s)
来源：http://iac.bjfxy.top

[S06] C：字符串比较
来源：http://sda.cqqwz.cn

strcmp(a, b) == 0
来源：http://nzr.cucudq.cn

[S07] C：数组遍历求和
来源：http://qwb.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cul.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://rwq.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yyf.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://ube.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qwf.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://wyv.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://nri.shzxlz.cn

[S11] C：逐行读文件
来源：http://kso.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://zbh.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oru.yuxming.cn

fclose(f);
来源：http://jjp.daria6918.cn

[S12] C：写文件
来源：http://cvu.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jbs.daria6918.cn

[S13] C：宏定义
来源：http://sbl.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pym.vqdsnc.cn

[S14] C：枚举
来源：http://ogg.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://ikz.andypj.xyz

[S15] C：类型转换
来源：http://dzy.zhijiandao.cn

(double) a / b
来源：http://zun.ehwqpu.com

[S16] C：位操作置位
来源：http://lxo.kuanghao11.cn

x |= (1 << 3);
来源：http://azc.cucudq.cn

[S17] C：安全拼接字符串
来源：http://ooj.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oci.hywenlv.cn

[S18] C：命令行参数
来源：http://sci.redwolf501.top

int main(int argc, char **argv)
来源：http://qnc.wangshuangyany.cn

[S19] C：快速排序
来源：http://xlg.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://wlv.aibaodan.cn

[S20] C：二分查找
来源：http://yxs.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://drx.yuxming.cn

[S21] C：字符类别判断
来源：http://uwr.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ttn.hammf.cn

[S22] C：字符串转数字
来源：http://aso.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://mjp.sxryk.cn

[S23] C：随机数
来源：http://tat.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cfj.epnwcf.com

[S24] C：获取本地时间
来源：http://gej.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ryk.cucudq.cn

[S25] C：内存拷贝
来源：http://arv.hammf.cn

memcpy(dst, src, n);
来源：http://qfp.haohaochexian.top

[S26] C：内存清零
来源：http://kkm.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://rnm.0kj1m.cn

[S27] C：定义常量
来源：http://ioe.zhixingplan.top

const double PI = 3.14159;
来源：http://dpl.iojbl.cn

[S28] C：静态变量
来源：http://enm.zhengqikj.top

static int counter = 0;
来源：http://nee.0kj1m.cn

[S29] C：变参函数
来源：http://tqx.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jty.smart0.xyz

[S30] C：头文件保护
来源：http://ejq.redwolf501.top

#ifndef X_H
来源：http://shn.cashguo.top

#define X_H
来源：http://wyi.xylfe.cn

#endif
来源：http://gxr.gogol.net.cn

[S31] C++：Hello World
来源：http://rce.c1oappe.top

#include <iostream>
来源：http://ibz.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://hjo.jqgfzy.top

[S32] C++：字符串
来源：http://ojw.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://btv.epnwcf.com

[S33] C++：vector 增删
来源：http://bpy.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ozm.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://khq.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://qoc.cheryme.top

[S35] C++：map
来源：http://kkf.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pab.jinqigfzy.top

[S36] C++：unordered_map
来源：http://tbf.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ucq.gaohongyu789.top

[S37] C++：set
来源：http://ezb.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tcq.haohaochexian.top

[S38] C++：排序
来源：http://jwp.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://mnt.zhengqikj.top

[S39] C++：自定义比较器排序
来源：http://zwf.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lpi.gogol.net.cn

[S40] C++：查找元素
来源：http://mgw.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gfn.epnwcf.com

[S41] C++：类与构造函数
来源：http://dvc.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aul.ybcxt.top

[S42] C++：继承与虚函数
来源：http://mow.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://oax.wangshuangyany.cn

[S43] C++：智能指针
来源：http://kdn.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://wzy.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://vnl.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://rzj.fzhhl.top

[S45] C++：lambda
来源：http://vij.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://kko.cdnleiting.top

[S46] C++：函数模板
来源：http://hnl.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lvk.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://iea.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gpb.daxiang520.top

[S48] C++：逐行读文件
来源：http://pwh.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ybr.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://gnz.fktsv.cn

[S49] C++：写文件
来源：http://wtj.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sgt.tarul.cn

[S50] C++：格式化数字
来源：http://wrs.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wbq.pycfn.com

[S51] C++：显式类型转换
来源：http://uxa.sysykeji.top

static_cast<double>(a) / b
来源：http://jaq.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://rbj.hnqzz.top

int size() const noexcept { return n_; }
来源：http://svy.aizwys.cn

[S53] C++：移动语义
来源：http://llf.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://ojn.jinqigufen.top

[S54] C++：异常处理
来源：http://ryf.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eze.daxiang520.top

[S55] C++：结构化绑定
来源：http://fxb.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bjz.xuanzx.com

[S56] C++：optional
来源：http://vmn.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oqr.yfazqb.com

[S57] C++：编译期常量
来源：http://nai.yvedp.cn

constexpr int N = 10;
来源：http://uvq.pycfn.com

[S58] C++：命名空间
来源：http://xyv.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://sfv.yangfankeji.com

[S59] C++：静态断言
来源：http://yph.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://idx.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://ncy.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wok.hcnkem.com

================================================================================
来源：http://kda.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jgo.fanxiaobao.xyz

================================================================================
来源：http://pjs.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://dju.hywenlv.cn

println("Hello")
来源：http://tgz.cdnleiting.top

[T02] Kotlin：变量
来源：http://bsq.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wnl.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://qzu.cashguo.top

"值: $b"
来源：http://sgb.jyoumei.cn

[T04] Kotlin：空安全
来源：http://qwy.xziqi.cn

val n: String? = null;  n?.length
来源：http://rzy.0kj1m.cn


<!-- 参考信息 -->