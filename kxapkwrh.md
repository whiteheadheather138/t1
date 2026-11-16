代发 wailian999

[Q78] 当前时间
来源：http://chq.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gld.aibaodan.cn

[Q79] 字符串拼接
来源：http://rej.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yev.yueranfly.top

[Q80] 字符串截取
来源：http://wij.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wcm.cqqwz.cn

[Q81] 字符串替换
来源：http://iba.cashguo.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zex.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://bgj.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nrb.yonumen.top

[Q83] 大小写转换
来源：http://zue.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qej.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://dkv.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://ysj.cashguo.top

[Q85] 数值取整
来源：http://kjp.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jur.jyoumei.cn

[Q86] 读取 JSON 字段
来源：http://rhq.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iqd.vehdjk.com

[Q87] JSON 字段做条件
来源：http://yud.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uol.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://qcv.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bpl.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bce.aizwys.cn

[Q89] 判断表是否存在
来源：http://ebs.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xgw.jinqigufen.top

[Q90] 生成序号列
来源：http://xil.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nhe.hysaishi.cn

================================================================================
来源：http://jcu.yfazqb.com

R. Bash 专题
来源：http://bqs.hfpthk.cn

================================================================================
来源：http://vxo.ehwqpu.com

[R01] shebang 与严格模式
来源：http://qod.yuxming.cn

#!/usr/bin/env bash
来源：http://efo.zhoulong.xyz

set -euo pipefail
来源：http://aig.hesvh.cn

[R02] 变量赋值与使用
来源：http://gvx.daria6918.cn

name="Tom"; echo "$name"
来源：http://brq.jqgufenzy.top

[R03] 只读变量
来源：http://yfz.fehbvm.com

readonly PI=3.14
来源：http://web.pycfn.com

[R04] 位置参数
来源：http://eym.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xvw.hnxiangtu.top

[R05] 参数默认值
来源：http://iav.yueranfly.top

name="${1:-default}"
来源：http://blg.tianlin.xyz

[R06] 判断命令是否存在
来源：http://ogw.jqgufenzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hiv.yangfankeji.com

[R07] if 判断文件
来源：http://iad.guannengcc.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qrr.jinqigufen.top

[R08] 数值比较
来源：http://ndf.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ihs.sjlbkw.cn

[R09] 字符串比较
来源：http://uvp.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rgl.nanxuanxn.top

[R10] 正则匹配
来源：http://qjw.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://arj.sufxvd.cn

[R11] case 多分支
来源：http://wol.chenlongwang.top

case "$1" in
来源：http://jbj.andypj.xyz

start) echo "启动" ;;
来源：http://ssc.svipenyu.cn

stop)  echo "停止" ;;
来源：http://wrw.xylfe.cn

*)     echo "未知命令" ;;
来源：http://evl.ppjwa.cn

esac
来源：http://wyg.andypj.xyz

[R12] for 遍历文件
来源：http://ecl.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://hkc.iojbl.cn

[R13] for 计数循环
来源：http://nxp.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://emn.sjlbkw.cn

[R14] C 风格 for
来源：http://ugh.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gxb.ydzc1.top

[R15] while 逐行读文件
来源：http://gem.nanxinkj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zjq.tanke756.top

[R16] until 等待条件
来源：http://ooo.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gbe.ivvv.top

[R17] 数组定义与取值
来源：http://tqe.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://utc.yuxming.cn

[R18] 遍历数组
来源：http://yfd.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tuu.yueranfly.top

[R19] 数组长度
来源：http://hux.kuanghao11.cn

echo "${#arr[@]}"
来源：http://cai.gzhubu.top

[R20] 关联数组（字典）
来源：http://udp.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ulu.shanyushiyangtech.top

[R21] 字符串长度
来源：http://wba.ydzc1.top

echo "${#s}"
来源：http://ukg.kuanghao11.cn

[R22] 截取子串
来源：http://cwl.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://tbd.wangdashe.top

[R23] 字符串替换
来源：http://krd.zhixingplan.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://orl.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://knm.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://ayr.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://xga.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://buj.xuanzx.com

[R26] 命令替换
来源：http://qkp.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://low.fktsv.cn

[R27] 算术展开
来源：http://ool.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://chk.dianchejie.cn

[R28] 浮点运算
来源：http://xxs.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://azt.yuxming.cn

[R29] 定义函数
来源：http://yxz.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dfy.cheryme.top

[R30] 函数返回状态码
来源：http://xok.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://ucj.zhijiandao.cn

[R31] 局部变量
来源：http://jys.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://pag.andypj.xyz

[R32] 参数个数校验
来源：http://ays.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nnm.yj20258.top

[R33] 捕获错误并提示行号
来源：http://kbr.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bhy.fzhhl.top

[R34] 退出时清理
来源：http://hne.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://kbz.ppjwa.cn

[R35] 后台执行并等待
来源：http://ozn.ivvv.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fop.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://zyk.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yqj.hcnkem.com

[R37] 把输出赋给变量
来源：http://dko.yanxiufei.cn

files=$(ls -1)
来源：http://qfr.nanxuanxn.top

[R38] 管道串联
来源：http://jcg.guannengcc.top

cat a.txt | grep -i error | wc -l
来源：http://nps.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://svw.guowangkeji.top

cmd > out.log 2>&1
来源：http://rut.guowangkeji.top

[R40] 追加写日志
来源：http://jvq.epnwcf.com

echo "log" >> out.log
来源：http://kxr.zycfv.cn

[R41] 丢弃输出
来源：http://goq.andypj.xyz

cmd >/dev/null 2>&1
来源：http://zlt.yongpay.top

[R42] 输入重定向
来源：http://jqi.316326.xyz

wc -l < a.txt
来源：http://ihq.hesvh.cn

[R43] 按名字查找文件
来源：http://zoy.mhx1999.top

find . -name "*.log" -type f
来源：http://tmr.epnwcf.com

[R44] 按修改时间查找
来源：http://ose.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://qbw.jiagoushi.top

[R45] 批量删除
来源：http://ayj.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://ljf.daxiang520.top

[R46] 递归替换文件内容
来源：http://njz.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iwm.birdmap.top

[R47] sed 单行替换
来源：http://hye.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://fvv.yuanzhike.top

[R48] awk 取指定列
来源：http://vtd.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://jqe.yfazqb.com

[R49] awk 带条件
来源：http://usx.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bmk.cheryme.top

[R50] awk 求和
来源：http://vuq.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xpn.shuidangran.top

[R51] 排序去重取前几
来源：http://mzr.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://mvi.epnwcf.com

[R52] 统计行数
来源：http://ncr.meibo888.top

wc -l a.txt
来源：http://tkd.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://dje.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://olo.iojbl.cn

[R54] 比较两个文件
来源：http://too.fzhhl.top

diff a.txt b.txt
来源：http://oyl.cdnleiting.top

[R55] 压缩与解压
来源：http://lxd.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jjh.wangshuangyany.cn

[R56] 远程拷贝
来源：http://xoc.xylfe.cn

scp file user@host:/path/
来源：http://atw.cucudq.cn

[R57] 远程执行命令
来源：http://had.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://zjc.xuanzx.com

[R58] 下载文件
来源：http://mvm.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://daa.nanxinkj.top

[R59] 发 POST JSON
来源：http://xak.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qov.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://zku.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hfm.yongpay.top

[R61] 磁盘占用
来源：http://bgp.yangfankeji.com

df -h;  du -sh *
来源：http://xvg.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://bth.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://tny.hongshengwenyu.top

[R63] 内存与进程
来源：http://ilk.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://rxw.yfazqb.com

[R64] 结束进程
来源：http://mag.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://zyx.nwbrower.top

[R65] 查看端口占用
来源：http://azj.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sju.hfpthk.cn

[R66] 定时任务
来源：http://uen.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://vsr.xinyue.icu

[R67] 生成随机十六进制串
来源：http://gtu.vqdsnc.cn

openssl rand -hex 16
来源：http://kfr.jinqigufen.top

[R68] 计算文件校验值
来源：http://gqo.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://vaz.zhoulong.xyz

[R69] 生成随机密码
来源：http://bbf.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://rqz.jinghuilouyu.cn

[R70] 时间戳与互转
来源：http://uyv.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://kev.mhx1999.top

[R71] 日期格式化
来源：http://fsb.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wlw.bbcook.cn

[R72] 等待端口就绪
来源：http://kkz.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xyk.fehbvm.com

[R73] 分割大日志
来源：http://gop.ydzc1.top

split -l 1000 big.log part_
来源：http://cxb.zhiwuduotai.top

[R74] 批量重命名
来源：http://sjd.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oqo.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://fjq.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://vdg.smart0.xyz

[R76] 使用临时文件
来源：http://yju.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sua.0kj1m.cn

[R77] 读取用户输入
来源：http://cvs.xziqi.cn

read -rp "请输入: " ans
来源：http://rkd.hesvh.cn

[R78] 交互式菜单
来源：http://nqo.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dgy.ehwqpu.com

[R79] 解析命令行选项
来源：http://iqx.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vxd.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://ejt.sufxvd.cn

time ./run.sh
来源：http://qjg.gogol.net.cn

================================================================================
来源：http://xwc.ehwqpu.com

S. C / C++ 专题
来源：http://rrb.kuanghao11.cn

================================================================================
来源：http://fxi.c1oappe.top

[S01] C：Hello World
来源：http://cjd.ydjk.org.cn

#include <stdio.h>
来源：http://qxu.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://rlc.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://ggp.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://sna.nwbrower.top

[S03] C：读入整数
来源：http://daf.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://htm.vehdjk.com

[S04] C：字符串复制
来源：http://phm.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://udj.yanxiufei.cn

[S05] C：字符串长度
来源：http://mks.dianchejie.cn

strlen(s)
来源：http://cev.hnxiangtu.top

[S06] C：字符串比较
来源：http://kts.yonumen.top

strcmp(a, b) == 0
来源：http://glh.guannengcc.top

[S07] C：数组遍历求和
来源：http://kpl.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sep.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://lgh.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lxb.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://gix.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://igm.meibo888.top

[S10] C：指针与解引用
来源：http://ftr.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://hcb.nanxinkj.top

[S11] C：逐行读文件
来源：http://zlm.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://ebz.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://lia.sxryk.cn

fclose(f);
来源：http://rsk.chenzaomai.com

[S12] C：写文件
来源：http://yzy.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jdp.9152youxi.cn

[S13] C：宏定义
来源：http://rzz.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wuk.sjlbkw.cn

[S14] C：枚举
来源：http://ujf.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://dnl.redwolf501.top

[S15] C：类型转换
来源：http://vtj.yfazqb.com

(double) a / b
来源：http://jzg.hnxiangtu.top

[S16] C：位操作置位
来源：http://umu.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://iuo.yueranfly.top

[S17] C：安全拼接字符串
来源：http://bsh.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sub.hnxiangtu.top

[S18] C：命令行参数
来源：http://bue.zdqjudy.top

int main(int argc, char **argv)
来源：http://lzv.xziqi.cn

[S19] C：快速排序
来源：http://cyn.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yji.tarul.cn

[S20] C：二分查找
来源：http://oyb.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iyd.ehwqpu.com

[S21] C：字符类别判断
来源：http://tgt.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://inm.xylfe.cn

[S22] C：字符串转数字
来源：http://mbj.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lwe.hnxiangtu.top

[S23] C：随机数
来源：http://dqi.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://but.vehdjk.com

[S24] C：获取本地时间
来源：http://dlo.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://twp.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://qeq.nanxuanxn.top

memcpy(dst, src, n);
来源：http://fzm.jqgufenzy.top

[S26] C：内存清零
来源：http://klj.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://qgi.hywenlv.cn

[S27] C：定义常量
来源：http://cvf.tanke756.top

const double PI = 3.14159;
来源：http://nyg.gotoacloud.top

[S28] C：静态变量
来源：http://vjn.iojbl.cn

static int counter = 0;
来源：http://zxi.shzxlz.cn

[S29] C：变参函数
来源：http://unh.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bwc.c1oappe.top

[S30] C：头文件保护
来源：http://aev.xziqi.cn

#ifndef X_H
来源：http://cvk.cqqwz.cn

#define X_H
来源：http://qmd.ybcxt.top

#endif
来源：http://ygk.zhiwuduotai.top

[S31] C++：Hello World
来源：http://uwl.nanxinkj.top

#include <iostream>
来源：http://iqf.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://dbt.ybcxt.top

[S32] C++：字符串
来源：http://tap.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://rdi.haohaochexian.top

[S33] C++：vector 增删
来源：http://qgj.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fse.hesvh.cn

[S34] C++：遍历 vector
来源：http://nzg.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://rfv.zhongyouzk.top

[S35] C++：map
来源：http://xwl.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nst.yueranfly.top

[S36] C++：unordered_map
来源：http://hgl.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://onu.yangfankeji.com

[S37] C++：set
来源：http://ket.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://etc.shanyushiyangtech.top

[S38] C++：排序
来源：http://iyk.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://ybq.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://sjz.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lwe.gogol.net.cn

[S40] C++：查找元素
来源：http://whd.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tlq.ydzc1.top

[S41] C++：类与构造函数
来源：http://lri.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kwj.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://hsx.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://utk.sweek.top

[S43] C++：智能指针
来源：http://ztq.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://gfw.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://aol.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://dkx.hfpthk.cn

[S45] C++：lambda
来源：http://prm.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://fxm.cheryme.top

[S46] C++：函数模板
来源：http://qox.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://amz.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://cec.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wbt.xylfe.cn

[S48] C++：逐行读文件
来源：http://iez.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://exm.smart0.xyz


<!-- 参考信息 -->