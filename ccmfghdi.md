代发 wailian999

[Q61] 移动平均
来源：http://rlj.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xvs.tian-w.cn

[Q62] 分组占比
来源：http://uzq.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dkf.zhixingplan.top

[Q63] 开启事务
来源：http://eru.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://asz.iojbl.cn

[Q64] 提交事务
来源：http://yzs.jyoumei.cn

COMMIT;
来源：http://pxn.fktsv.cn

[Q65] 回滚事务
来源：http://xqd.yfazqb.com

ROLLBACK;
来源：http://spd.xziqi.cn

[Q66] 行锁查询
来源：http://baf.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ocl.cdnleiting.top

[Q67] 设置隔离级别
来源：http://kkw.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://huk.yangfankeji.com

[Q68] 保存点
来源：http://okx.yongpay.top

SAVEPOINT sp1;
来源：http://vtu.tian-w.cn

ROLLBACK TO sp1;
来源：http://hav.zhixingplan.top

[Q69] 查看执行计划
来源：http://bsf.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iiw.jinghuilouyu.cn

[Q70] 更新统计信息
来源：http://xaf.gaohongyu789.top

ANALYZE TABLE users;
来源：http://kxh.tianlin.xyz

[Q71] 查看建表语句
来源：http://tvj.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xps.c1oappe.top

[Q72] 查看索引
来源：http://xue.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://uvd.iojbl.cn

[Q73] 查看表状态
来源：http://lyk.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://roe.tarul.cn

[Q74] 强制使用索引
来源：http://pqi.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nep.pengpengdd.cyou

[Q75] 日期格式化
来源：http://ile.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hoz.gotoacloud.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aku.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://lhb.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yek.zhengqikj.top

[Q77] 时间加减
来源：http://qsk.bjfxy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://viq.haohaochexian.top

[Q78] 当前时间
来源：http://jxk.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dwi.aizwys.cn

[Q79] 字符串拼接
来源：http://egb.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qyz.nanxinkj.top

[Q80] 字符串截取
来源：http://htl.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jrk.zdbjq.cn

[Q81] 字符串替换
来源：http://woz.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zps.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://ver.yanxiufei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aky.yonumen.top

[Q83] 大小写转换
来源：http://mhl.tarul.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ceo.xinyue.icu

[Q84] 去除首尾空格
来源：http://upz.yuxming.cn

SELECT TRIM(name) FROM users;
来源：http://syv.gogol.net.cn

[Q85] 数值取整
来源：http://hvc.sxryk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zzq.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://kwx.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://obu.cucudq.cn

[Q87] JSON 字段做条件
来源：http://lry.ivvv.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ggb.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://niz.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ysl.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fpi.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://gwp.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://irc.zhiwuduotai.top

[Q90] 生成序号列
来源：http://quw.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://byj.jqgufenzy.top

================================================================================
来源：http://wpw.cashguo.top

R. Bash 专题
来源：http://mcr.svipenyu.cn

================================================================================
来源：http://yuo.9152youxi.cn

[R01] shebang 与严格模式
来源：http://itl.jyoumei.cn

#!/usr/bin/env bash
来源：http://pqg.jianghu66.top

set -euo pipefail
来源：http://lsm.ydjk.org.cn

[R02] 变量赋值与使用
来源：http://bre.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://pcj.tarul.cn

[R03] 只读变量
来源：http://ape.zdqjudy.top

readonly PI=3.14
来源：http://yqv.fanxiaobao.xyz

[R04] 位置参数
来源：http://hnq.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xir.ivvv.top

[R05] 参数默认值
来源：http://bej.ywan-chungtsiang.top

name="${1:-default}"
来源：http://zml.0kj1m.cn

[R06] 判断命令是否存在
来源：http://sjm.0kj1m.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fsw.ivvv.top

[R07] if 判断文件
来源：http://dom.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://usr.zhiwuduotai.top

[R08] 数值比较
来源：http://vbx.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tfq.fzhhl.top

[R09] 字符串比较
来源：http://vwu.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vkp.zhixingplan.top

[R10] 正则匹配
来源：http://mhg.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ywu.birdmap.top

[R11] case 多分支
来源：http://una.hesvh.cn

case "$1" in
来源：http://gvo.jqgufenzy.top

start) echo "启动" ;;
来源：http://zmj.cheryme.top

stop)  echo "停止" ;;
来源：http://qvo.sjlbkw.cn

*)     echo "未知命令" ;;
来源：http://rcx.nwbrower.top

esac
来源：http://dky.hnxiangtu.top

[R12] for 遍历文件
来源：http://dnx.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://dvp.zhoulong.xyz

[R13] for 计数循环
来源：http://eoo.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://jdi.xuanzx.com

[R14] C 风格 for
来源：http://evc.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rsh.hcnkem.com

[R15] while 逐行读文件
来源：http://yuc.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vyq.xziqi.cn

[R16] until 等待条件
来源：http://ael.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mmx.316326.xyz

[R17] 数组定义与取值
来源：http://yvq.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wai.jinghuilouyu.cn

[R18] 遍历数组
来源：http://ijc.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iei.hysaishi.cn

[R19] 数组长度
来源：http://isi.bbcook.cn

echo "${#arr[@]}"
来源：http://znw.sxryk.cn

[R20] 关联数组（字典）
来源：http://mft.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://amd.ivvv.top

[R21] 字符串长度
来源：http://kxr.zhaomingkeji.xyz

echo "${#s}"
来源：http://pqx.ydzc1.top

[R22] 截取子串
来源：http://gny.iojbl.cn

echo "${s:0:5}"
来源：http://dzj.jinqigfzy.top

[R23] 字符串替换
来源：http://jkv.ivvv.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fpo.c1oappe.top

[R24] 大小写转换
来源：http://dvw.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dce.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://sfn.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xuw.fehbvm.com

[R26] 命令替换
来源：http://wxh.zhixingplan.top

now=$(date +%F); echo "$now"
来源：http://qmc.haohaochexian.top

[R27] 算术展开
来源：http://wrf.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://eta.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://ynz.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://hpq.andypj.xyz

[R29] 定义函数
来源：http://cfm.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zga.jqgfzy.top

[R30] 函数返回状态码
来源：http://mfc.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://fxq.havefunace.top

[R31] 局部变量
来源：http://ikb.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://avt.sysykeji.top

[R32] 参数个数校验
来源：http://cig.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sdt.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://ooy.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rpr.hywenlv.cn

[R34] 退出时清理
来源：http://nmr.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://arm.xinyue.icu

[R35] 后台执行并等待
来源：http://iex.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://afx.hcnkem.com

[R36] 并发执行多个任务
来源：http://qbd.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nlu.bbcook.cn

[R37] 把输出赋给变量
来源：http://gkj.sysykeji.top

files=$(ls -1)
来源：http://sdg.yuxming.cn

[R38] 管道串联
来源：http://gub.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://hag.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://qju.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://ixf.bbcook.cn

[R40] 追加写日志
来源：http://cms.tarul.cn

echo "log" >> out.log
来源：http://asp.mhx1999.top

[R41] 丢弃输出
来源：http://lgq.xinyue.icu

cmd >/dev/null 2>&1
来源：http://ypy.tianlin.xyz

[R42] 输入重定向
来源：http://lbo.shuidangran.top

wc -l < a.txt
来源：http://qzd.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://xsv.birdmap.top

find . -name "*.log" -type f
来源：http://lma.ydzc1.top

[R44] 按修改时间查找
来源：http://whl.yongpay.top

find . -mtime -7 -type f
来源：http://bhg.sweek.top

[R45] 批量删除
来源：http://gzs.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://xaf.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://hco.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gnl.hesvh.cn

[R47] sed 单行替换
来源：http://vyb.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://mvk.hcnkem.com

[R48] awk 取指定列
来源：http://dzl.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://mhu.zhongyouzk.top

[R49] awk 带条件
来源：http://hpf.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bms.zdbjq.cn

[R50] awk 求和
来源：http://jzs.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://kbg.yj20258.top

[R51] 排序去重取前几
来源：http://qeq.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wbb.shanyushiyangtech.top

[R52] 统计行数
来源：http://yue.cdnleiting.top

wc -l a.txt
来源：http://qoj.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://uvm.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qiv.zdbjq.cn

[R54] 比较两个文件
来源：http://sxh.jlsjyb.cn

diff a.txt b.txt
来源：http://ajn.hnxiangtu.top

[R55] 压缩与解压
来源：http://ysa.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qyl.nwbrower.top

[R56] 远程拷贝
来源：http://otv.shangyingyoupin.top

scp file user@host:/path/
来源：http://vso.havefunace.top

[R57] 远程执行命令
来源：http://djj.gogol.net.cn

ssh user@host 'uptime'
来源：http://uzd.hammf.cn

[R58] 下载文件
来源：http://bmz.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xnc.hysaishi.cn

[R59] 发 POST JSON
来源：http://jfo.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vge.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://uco.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lxk.zhiwuduotai.top

[R61] 磁盘占用
来源：http://rhj.svipenyu.cn

df -h;  du -sh *
来源：http://mdn.ivvv.top

[R62] 找最占空间的文件
来源：http://dxi.meibo888.top

du -ah . | sort -rh | head -10
来源：http://did.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://oid.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://mhf.yangfankeji.com

[R64] 结束进程
来源：http://cgy.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://obc.jianghu66.top

[R65] 查看端口占用
来源：http://nip.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yva.daria6918.cn

[R66] 定时任务
来源：http://ioe.xuanzx.com

crontab -e;  crontab -l
来源：http://jyu.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://whj.cucudq.cn

openssl rand -hex 16
来源：http://pqw.jyoumei.cn

[R68] 计算文件校验值
来源：http://jjn.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://duo.iojbl.cn

[R69] 生成随机密码
来源：http://vkx.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://nwk.52xcode.cn

[R70] 时间戳与互转
来源：http://bjt.ydzc1.top

date +%s;  date -d @1700000000
来源：http://wgc.tanke756.top

[R71] 日期格式化
来源：http://mix.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yax.bjfxy.top

[R72] 等待端口就绪
来源：http://rci.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://esh.zdqjudy.top

[R73] 分割大日志
来源：http://oeg.bbcook.cn

split -l 1000 big.log part_
来源：http://izg.hysaishi.cn

[R74] 批量重命名
来源：http://wqi.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://snd.fzhhl.top

[R75] 导出环境变量
来源：http://cij.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://jru.kuanghao11.cn

[R76] 使用临时文件
来源：http://qya.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://glp.hnqzz.top

[R77] 读取用户输入
来源：http://vlr.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://pnh.dianchejie.cn

[R78] 交互式菜单
来源：http://skx.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ctq.ctjpmb.com

[R79] 解析命令行选项
来源：http://njd.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://exq.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://xrn.yuanzhike.top

time ./run.sh
来源：http://ogq.dianchejie.cn

================================================================================
来源：http://epc.daxiang520.top

S. C / C++ 专题
来源：http://euv.jianghu66.top

================================================================================
来源：http://tli.nanxinkj.top

[S01] C：Hello World
来源：http://rcx.jinqigfzy.top

#include <stdio.h>
来源：http://hhj.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qth.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://wxd.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://nhu.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://wne.ybcxt.top

int x; scanf("%d", &x);
来源：http://epy.0kj1m.cn

[S04] C：字符串复制
来源：http://kjh.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://ufq.xinyue.icu

[S05] C：字符串长度
来源：http://grn.ydzc1.top

strlen(s)
来源：http://dms.jinqigfzy.top

[S06] C：字符串比较
来源：http://mpw.chenlongwang.top

strcmp(a, b) == 0
来源：http://rvt.yueranfly.top

[S07] C：数组遍历求和
来源：http://wnk.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vnx.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://lin.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jyp.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://wpm.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nrs.jinqigufen.top

[S10] C：指针与解引用
来源：http://llf.yj202588.top

int *p = &a;  *p = 5;
来源：http://cce.tian-w.cn

[S11] C：逐行读文件
来源：http://itt.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://vcf.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pyl.wangdashe.top

fclose(f);
来源：http://qtg.cheryme.top

[S12] C：写文件
来源：http://piw.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pdn.gotoacloud.top

[S13] C：宏定义
来源：http://tlz.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qjy.fehbvm.com

[S14] C：枚举
来源：http://kym.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ony.xuanzx.com

[S15] C：类型转换
来源：http://mqb.zdbjq.cn

(double) a / b
来源：http://hyn.jinqigfzy.top

[S16] C：位操作置位
来源：http://vtz.cucudq.cn

x |= (1 << 3);
来源：http://ncc.daria6918.cn

[S17] C：安全拼接字符串
来源：http://qdt.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pmo.yongpay.top

[S18] C：命令行参数
来源：http://mqs.fzhhl.top

int main(int argc, char **argv)
来源：http://atl.havefunace.top

[S19] C：快速排序
来源：http://joy.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tih.guannengcc.top

[S20] C：二分查找
来源：http://uyq.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sqj.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://edo.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://soh.guowangkeji.top

[S22] C：字符串转数字
来源：http://xws.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://jyx.smart0.xyz

[S23] C：随机数
来源：http://gae.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xgl.redwolf501.top

[S24] C：获取本地时间
来源：http://zlu.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://npg.cheryme.top

[S25] C：内存拷贝
来源：http://hpk.zycfv.cn

memcpy(dst, src, n);
来源：http://zeu.tarul.cn

[S26] C：内存清零
来源：http://dix.sxryk.cn

memset(a, 0, sizeof a);
来源：http://bbf.hcnkem.com

[S27] C：定义常量
来源：http://olk.ydzc1.top

const double PI = 3.14159;
来源：http://wbi.gaohongyu789.top

[S28] C：静态变量
来源：http://pfe.0kj1m.cn

static int counter = 0;
来源：http://ivw.ydzc1.top

[S29] C：变参函数
来源：http://qhb.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jtp.cheryme.top

[S30] C：头文件保护
来源：http://ycf.bjfxy.top

#ifndef X_H
来源：http://ddu.wangdashe.top

#define X_H
来源：http://jur.mhx1999.top

#endif
来源：http://uog.shuidangran.top

[S31] C++：Hello World
来源：http://yky.ywan-chungtsiang.top


<!-- 参考信息 -->