代发 wailian999

SHOW INDEX FROM users;
来源：http://zot.ydjk.org.cn

[Q73] 查看表状态
来源：http://pcy.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rsx.zhengqikj.top

[Q74] 强制使用索引
来源：http://dwy.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://llf.52xcode.cn

[Q75] 日期格式化
来源：http://jaw.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jqc.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pit.fktsv.cn

[Q76] 按天统计
来源：http://tua.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tzf.mhx1999.top

[Q77] 时间加减
来源：http://tuq.gotoacloud.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rci.snrcjt.cn

[Q78] 当前时间
来源：http://spg.yvedp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dsa.mhx1999.top

[Q79] 字符串拼接
来源：http://gtl.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xrt.wangshuangyany.cn

[Q80] 字符串截取
来源：http://lva.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rfn.zdbjq.cn

[Q81] 字符串替换
来源：http://ric.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rvr.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://pch.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pej.daria6918.cn

[Q83] 大小写转换
来源：http://woi.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qlh.redwolf501.top

[Q84] 去除首尾空格
来源：http://hum.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://pam.feifeiyinyue.top

[Q85] 数值取整
来源：http://aom.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ett.yongpay.top

[Q86] 读取 JSON 字段
来源：http://pia.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://thm.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://dqz.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://asy.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://gfn.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zjw.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://woy.xziqi.cn

[Q89] 判断表是否存在
来源：http://nfy.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ilr.yanxiufei.cn

[Q90] 生成序号列
来源：http://ieo.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wqb.chenjidiqi.icu

================================================================================
来源：http://jgf.chenzaomai.com

R. Bash 专题
来源：http://lfi.zhoulong.xyz

================================================================================
来源：http://ive.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://rmh.andypj.xyz

#!/usr/bin/env bash
来源：http://zzt.andypj.xyz

set -euo pipefail
来源：http://oyb.aibaodan.cn

[R02] 变量赋值与使用
来源：http://bvf.fanxiaobao.xyz

name="Tom"; echo "$name"
来源：http://bgt.cdnleiting.top

[R03] 只读变量
来源：http://dai.shuidangran.top

readonly PI=3.14
来源：http://jxv.hnxiangtu.top

[R04] 位置参数
来源：http://neo.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cwl.daria6918.cn

[R05] 参数默认值
来源：http://rhf.zdqjudy.top

name="${1:-default}"
来源：http://ija.fktsv.cn

[R06] 判断命令是否存在
来源：http://mnw.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zyw.tanke756.top

[R07] if 判断文件
来源：http://rtu.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pou.pengpengdd.cyou

[R08] 数值比较
来源：http://hut.wangdashe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qjr.jinyuanbaomall.cn

[R09] 字符串比较
来源：http://onv.xuetiantiany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uzo.sufxvd.cn

[R10] 正则匹配
来源：http://dei.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cms.fktsv.cn

[R11] case 多分支
来源：http://nth.daria6918.cn

case "$1" in
来源：http://mpv.hfpthk.cn

start) echo "启动" ;;
来源：http://eoq.9152youxi.cn

stop)  echo "停止" ;;
来源：http://xmb.bbcook.cn

*)     echo "未知命令" ;;
来源：http://zmn.aizwys.cn

esac
来源：http://udq.fehbvm.com

[R12] for 遍历文件
来源：http://shm.jqgfzy.top

for f in *.txt; do echo "$f"; done
来源：http://viv.ctjpmb.com

[R13] for 计数循环
来源：http://nnn.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://tlo.zhiwuduotai.top

[R14] C 风格 for
来源：http://duw.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fgv.yanxiufei.cn

[R15] while 逐行读文件
来源：http://xpf.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ctj.dianchejie.cn

[R16] until 等待条件
来源：http://dpg.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gya.xylfe.cn

[R17] 数组定义与取值
来源：http://qpx.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://tce.xziqi.cn

[R18] 遍历数组
来源：http://exs.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ezv.wangdashe.top

[R19] 数组长度
来源：http://ydm.aizwys.cn

echo "${#arr[@]}"
来源：http://wxl.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://swg.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zjz.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://mvf.daxiang520.top

echo "${#s}"
来源：http://pzr.xylfe.cn

[R22] 截取子串
来源：http://ozu.wangshuangyany.cn

echo "${s:0:5}"
来源：http://knl.sweek.top

[R23] 字符串替换
来源：http://ggc.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://laf.redwolf501.top

[R24] 大小写转换
来源：http://cgo.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://cmb.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://rxa.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hwr.vehdjk.com

[R26] 命令替换
来源：http://dxs.birdmap.top

now=$(date +%F); echo "$now"
来源：http://jrd.shangyingyoupin.top

[R27] 算术展开
来源：http://lhh.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://rvi.daria6918.cn

[R28] 浮点运算
来源：http://kud.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://hoq.birdmap.top

[R29] 定义函数
来源：http://yfn.yongpay.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iuo.meibo888.top

[R30] 函数返回状态码
来源：http://frm.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://vgz.jinghuilouyu.cn

[R31] 局部变量
来源：http://lmp.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://wdg.zycfv.cn

[R32] 参数个数校验
来源：http://eil.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://egr.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://iru.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://weo.ivvv.top

[R34] 退出时清理
来源：http://sqm.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://fyz.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://jmh.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bnk.daxiang520.top

[R36] 并发执行多个任务
来源：http://zio.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fui.yuxming.cn

[R37] 把输出赋给变量
来源：http://yye.fktsv.cn

files=$(ls -1)
来源：http://wed.hnqzz.top

[R38] 管道串联
来源：http://jiw.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://cpt.yj202588.top

[R39] 重定向标准输出与错误
来源：http://dgg.redwolf501.top

cmd > out.log 2>&1
来源：http://jzi.pengpengdd.cyou

[R40] 追加写日志
来源：http://vgo.hnqzz.top

echo "log" >> out.log
来源：http://squ.cdnleiting.top

[R41] 丢弃输出
来源：http://tqc.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://qvb.jinqigfzy.top

[R42] 输入重定向
来源：http://ued.yj20258.top

wc -l < a.txt
来源：http://mtj.yuxming.cn

[R43] 按名字查找文件
来源：http://eee.yj20258888.top

find . -name "*.log" -type f
来源：http://fas.yfazqb.com

[R44] 按修改时间查找
来源：http://thb.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://swf.pengpengdd.cyou

[R45] 批量删除
来源：http://azo.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://ntz.fzhhl.top

[R46] 递归替换文件内容
来源：http://rjj.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cwu.tianlin.xyz

[R47] sed 单行替换
来源：http://ejj.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://klu.yj202588.top

[R48] awk 取指定列
来源：http://xxr.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://gdq.zhijiandao.cn

[R49] awk 带条件
来源：http://aoz.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cjb.aibaodan.cn

[R50] awk 求和
来源：http://lpq.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://chy.hywenlv.cn

[R51] 排序去重取前几
来源：http://gbq.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wxd.yueranfly.top

[R52] 统计行数
来源：http://xyq.ctjpmb.com

wc -l a.txt
来源：http://unu.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://miw.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://byu.svipenyu.cn

[R54] 比较两个文件
来源：http://vlc.vehdjk.com

diff a.txt b.txt
来源：http://lcp.fengsongda.top

[R55] 压缩与解压
来源：http://kog.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://isz.meibo888.top

[R56] 远程拷贝
来源：http://dce.nanxuanxn.top

scp file user@host:/path/
来源：http://kte.nanxinkj.top

[R57] 远程执行命令
来源：http://qet.jianghu66.top

ssh user@host 'uptime'
来源：http://wnn.yonumen.top

[R58] 下载文件
来源：http://ger.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mup.svipenyu.cn

[R59] 发 POST JSON
来源：http://kie.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cfe.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://pll.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tzz.chenjidiqi.icu

[R61] 磁盘占用
来源：http://avv.daxiang520.top

df -h;  du -sh *
来源：http://xrp.yj202588.top

[R62] 找最占空间的文件
来源：http://jpy.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://mjj.hcnkem.com

[R63] 内存与进程
来源：http://lpp.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://edg.cashguo.top

[R64] 结束进程
来源：http://rnb.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://vix.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://rmw.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jec.yuxming.cn

[R66] 定时任务
来源：http://guu.jlsjyb.cn

crontab -e;  crontab -l
来源：http://zdt.yj20258888.top

[R67] 生成随机十六进制串
来源：http://pzo.bbcook.cn

openssl rand -hex 16
来源：http://ffb.smart0.xyz

[R68] 计算文件校验值
来源：http://vud.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eux.vqdsnc.cn

[R69] 生成随机密码
来源：http://ydd.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://vmp.haohaochexian.top

[R70] 时间戳与互转
来源：http://ycw.sysykeji.top

date +%s;  date -d @1700000000
来源：http://qwp.andypj.xyz

[R71] 日期格式化
来源：http://shm.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://avd.aizwys.cn

[R72] 等待端口就绪
来源：http://otn.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://isj.tian-w.cn

[R73] 分割大日志
来源：http://igi.sysykeji.top

split -l 1000 big.log part_
来源：http://bju.andypj.xyz

[R74] 批量重命名
来源：http://dls.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uoo.zhijiandao.cn

[R75] 导出环境变量
来源：http://qtj.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://diy.iojbl.cn

[R76] 使用临时文件
来源：http://jzz.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ydi.ydjk.org.cn

[R77] 读取用户输入
来源：http://ahk.zdbjq.cn

read -rp "请输入: " ans
来源：http://nsf.sufxvd.cn

[R78] 交互式菜单
来源：http://szj.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kdp.hesvh.cn

[R79] 解析命令行选项
来源：http://pyv.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://coj.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://knh.hesvh.cn

time ./run.sh
来源：http://rgv.fzhhl.top

================================================================================
来源：http://zmp.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://yzt.yvedp.cn

================================================================================
来源：http://etd.hnxiangtu.top

[S01] C：Hello World
来源：http://avt.ivvv.top

#include <stdio.h>
来源：http://fbx.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wey.nwbrower.top

[S02] C：变量与格式化输出
来源：http://von.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://jyw.zhijiandao.cn

[S03] C：读入整数
来源：http://xqc.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://fet.shuidangran.top

[S04] C：字符串复制
来源：http://gnx.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ljp.hnxiangtu.top

[S05] C：字符串长度
来源：http://saf.xuanzx.com

strlen(s)
来源：http://pzl.pycfn.com

[S06] C：字符串比较
来源：http://adw.tanke756.top

strcmp(a, b) == 0
来源：http://nhb.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://omj.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bpn.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://hpc.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ghq.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://ppm.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://otl.yuxming.cn

[S10] C：指针与解引用
来源：http://wsr.gzhubu.top

int *p = &a;  *p = 5;
来源：http://eyq.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://jqn.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://hsh.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nhi.hywenlv.cn

fclose(f);
来源：http://vew.yvedp.cn

[S12] C：写文件
来源：http://rkt.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://czd.vehdjk.com

[S13] C：宏定义
来源：http://tlz.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pvt.yueranfly.top

[S14] C：枚举
来源：http://pkv.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://yyk.zycfv.cn

[S15] C：类型转换
来源：http://uux.ywan-chungtsiang.top

(double) a / b
来源：http://bri.birdmap.top

[S16] C：位操作置位
来源：http://eae.ppjwa.cn

x |= (1 << 3);
来源：http://bhe.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://ens.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://etj.xylfe.cn

[S18] C：命令行参数
来源：http://url.iojbl.cn

int main(int argc, char **argv)
来源：http://fbb.hcnkem.com

[S19] C：快速排序
来源：http://jap.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://nup.zhixingplan.top

[S20] C：二分查找
来源：http://kxd.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sqb.hfpthk.cn

[S21] C：字符类别判断
来源：http://hwi.zhengqikj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ktu.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://jsa.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://bft.nanxuanxn.top

[S23] C：随机数
来源：http://lje.cqqwz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dvc.yonumen.top

[S24] C：获取本地时间
来源：http://ead.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nby.smart0.xyz

[S25] C：内存拷贝
来源：http://lnn.quarkkingdee.top

memcpy(dst, src, n);
来源：http://inc.bjfxy.top

[S26] C：内存清零
来源：http://how.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://lil.jinqigufen.top

[S27] C：定义常量
来源：http://yls.yonumen.top

const double PI = 3.14159;
来源：http://nys.ydzc1.top

[S28] C：静态变量
来源：http://adw.svipenyu.cn

static int counter = 0;
来源：http://fjh.ehwqpu.com

[S29] C：变参函数
来源：http://fms.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kmv.yonumen.top

[S30] C：头文件保护
来源：http://mrn.ctjpmb.com

#ifndef X_H
来源：http://mxo.guowangkeji.top

#define X_H
来源：http://vtr.ctjpmb.com

#endif
来源：http://gap.svipenyu.cn

[S31] C++：Hello World
来源：http://cof.gotoacloud.top

#include <iostream>
来源：http://wgg.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://atw.guowangkeji.top

[S32] C++：字符串
来源：http://cfb.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://wdc.mhx1999.top

[S33] C++：vector 增删
来源：http://pqi.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dnb.yj202588.top

[S34] C++：遍历 vector
来源：http://fxk.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://hnw.cdnleiting.top

[S35] C++：map
来源：http://fiy.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://soe.ppjwa.cn

[S36] C++：unordered_map
来源：http://eqw.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jeg.wangdashe.top

[S37] C++：set
来源：http://nvt.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eto.yuanzhike.top

[S38] C++：排序
来源：http://qit.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://stw.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://hfp.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xqt.cqqwz.cn

[S40] C++：查找元素
来源：http://zzi.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://acm.bjfxy.top

[S41] C++：类与构造函数
来源：http://pny.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gob.aizwys.cn

[S42] C++：继承与虚函数
来源：http://efz.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://iho.yj202588.top


<!-- 参考信息 -->