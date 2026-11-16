代发 wailian999

[Q61] 移动平均
来源：http://egz.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jjr.xuanzx.com

[Q62] 分组占比
来源：http://wan.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lit.jiagoushi.top

[Q63] 开启事务
来源：http://bzs.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dkb.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://jyo.guannengcc.top

COMMIT;
来源：http://bvl.tian-w.cn

[Q65] 回滚事务
来源：http://gxw.zhengqikj.top

ROLLBACK;
来源：http://cip.ybcxt.top

[Q66] 行锁查询
来源：http://msj.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hxm.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://kiu.yueranfly.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oqo.hcnkem.com

[Q68] 保存点
来源：http://wcr.ppjwa.cn

SAVEPOINT sp1;
来源：http://pek.yuxming.cn

ROLLBACK TO sp1;
来源：http://ldg.meibo888.top

[Q69] 查看执行计划
来源：http://rze.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mbn.smart0.xyz

[Q70] 更新统计信息
来源：http://mab.jinghuilouyu.cn

ANALYZE TABLE users;
来源：http://ovc.yanxiufei.cn

[Q71] 查看建表语句
来源：http://tkm.iojbl.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hxg.9152youxi.cn

[Q72] 查看索引
来源：http://snc.hysaishi.cn

SHOW INDEX FROM users;
来源：http://nwp.snrcjt.cn

[Q73] 查看表状态
来源：http://ljg.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pat.bjfxy.top

[Q74] 强制使用索引
来源：http://dbf.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pux.ybcxt.top

[Q75] 日期格式化
来源：http://jqz.jlsjyb.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://buh.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ssg.hywenlv.cn

[Q76] 按天统计
来源：http://arj.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qqo.fzhhl.top

[Q77] 时间加减
来源：http://ayo.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zsh.hammf.cn

[Q78] 当前时间
来源：http://gsq.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jzu.cqqwz.cn

[Q79] 字符串拼接
来源：http://jqg.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://emq.bbcook.cn

[Q80] 字符串截取
来源：http://fgj.ybcxt.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ote.fehbvm.com

[Q81] 字符串替换
来源：http://dis.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ezn.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://iny.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eut.chenzaomai.com

[Q83] 大小写转换
来源：http://tjo.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dmb.jqgfzy.top

[Q84] 去除首尾空格
来源：http://vds.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://bmo.hnxiangtu.top

[Q85] 数值取整
来源：http://xny.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yeu.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://ejp.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://scs.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://trj.yuanzhike.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oai.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://uyf.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xzo.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qpq.ybcxt.top

[Q89] 判断表是否存在
来源：http://hxh.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://swg.redwolf501.top

[Q90] 生成序号列
来源：http://yii.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ozm.fanxiaobao.xyz

================================================================================
来源：http://uzh.pengpengdd.cyou

R. Bash 专题
来源：http://njr.shuidangran.top

================================================================================
来源：http://tiu.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://znh.xinyue.icu

#!/usr/bin/env bash
来源：http://wds.hesvh.cn

set -euo pipefail
来源：http://lja.yuxming.cn

[R02] 变量赋值与使用
来源：http://nyl.hesvh.cn

name="Tom"; echo "$name"
来源：http://dis.jqgfzy.top

[R03] 只读变量
来源：http://sck.ehwqpu.com

readonly PI=3.14
来源：http://kud.wangdashe.top

[R04] 位置参数
来源：http://gus.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mrt.jqgufenzy.top

[R05] 参数默认值
来源：http://yjw.tian-w.cn

name="${1:-default}"
来源：http://cpu.smart0.xyz

[R06] 判断命令是否存在
来源：http://vbk.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cmw.yj20258.top

[R07] if 判断文件
来源：http://fpw.fengsongda.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xrg.yj20258888.top

[R08] 数值比较
来源：http://aio.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://gus.shzxlz.cn

[R09] 字符串比较
来源：http://gic.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xyd.feifeiyinyue.top

[R10] 正则匹配
来源：http://cpg.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://svc.shangyingyoupin.top

[R11] case 多分支
来源：http://utv.guowangkeji.top

case "$1" in
来源：http://pjq.yangfankeji.com

start) echo "启动" ;;
来源：http://lni.iojbl.cn

stop)  echo "停止" ;;
来源：http://pak.gzhubu.top

*)     echo "未知命令" ;;
来源：http://oji.sweek.top

esac
来源：http://kwy.tian-w.cn

[R12] for 遍历文件
来源：http://lsb.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://vjc.ppjwa.cn

[R13] for 计数循环
来源：http://kmh.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://bgy.birdmap.top

[R14] C 风格 for
来源：http://flu.vqdsnc.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pem.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://wbl.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ish.feifeiyinyue.top

[R16] until 等待条件
来源：http://yec.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://opy.chenzaomai.com

[R17] 数组定义与取值
来源：http://ncp.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://vvw.daxiang520.top

[R18] 遍历数组
来源：http://tij.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jki.bjfxy.top

[R19] 数组长度
来源：http://fkm.daria6918.cn

echo "${#arr[@]}"
来源：http://eim.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://mac.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rkz.jlsjyb.cn

[R21] 字符串长度
来源：http://mbr.haohaochexian.top

echo "${#s}"
来源：http://fur.meibo888.top

[R22] 截取子串
来源：http://lcp.pycfn.com

echo "${s:0:5}"
来源：http://tyr.cqqwz.cn

[R23] 字符串替换
来源：http://nle.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jru.gogol.net.cn

[R24] 大小写转换
来源：http://tww.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lvj.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://yvo.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mgn.cucudq.cn

[R26] 命令替换
来源：http://nlh.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://rcx.iojbl.cn

[R27] 算术展开
来源：http://kju.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://nah.sweek.top

[R28] 浮点运算
来源：http://blf.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://nvz.jinyuanbaomall.cn

[R29] 定义函数
来源：http://ydb.c1oappe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gef.yangfankeji.com

[R30] 函数返回状态码
来源：http://esy.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://mzd.yvedp.cn

[R31] 局部变量
来源：http://yex.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://jmm.sweek.top

[R32] 参数个数校验
来源：http://kdb.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lbt.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://cpq.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fry.c1oappe.top

[R34] 退出时清理
来源：http://cpe.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://dto.redwolf501.top

[R35] 后台执行并等待
来源：http://owb.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wre.yonumen.top

[R36] 并发执行多个任务
来源：http://qfc.svipenyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pfv.sxryk.cn

[R37] 把输出赋给变量
来源：http://mmu.zhijiandao.cn

files=$(ls -1)
来源：http://qso.jqgfzy.top

[R38] 管道串联
来源：http://lht.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://cyr.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://fhb.jinqigfzy.top

cmd > out.log 2>&1
来源：http://lwe.9152youxi.cn

[R40] 追加写日志
来源：http://jmw.hesvh.cn

echo "log" >> out.log
来源：http://aos.cashguo.top

[R41] 丢弃输出
来源：http://vjv.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://ozq.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://gci.aibaodan.cn

wc -l < a.txt
来源：http://tzk.xinyue.icu

[R43] 按名字查找文件
来源：http://mod.52xcode.cn

find . -name "*.log" -type f
来源：http://ddf.tarul.cn

[R44] 按修改时间查找
来源：http://vpo.ppjwa.cn

find . -mtime -7 -type f
来源：http://sda.chenlongwang.top

[R45] 批量删除
来源：http://ben.epnwcf.com

find . -name "*.tmp" -delete
来源：http://vko.jqgfzy.top

[R46] 递归替换文件内容
来源：http://swp.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gvr.yfazqb.com

[R47] sed 单行替换
来源：http://wph.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://idc.sxryk.cn

[R48] awk 取指定列
来源：http://cfm.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://lvk.0kj1m.cn

[R49] awk 带条件
来源：http://hxo.shangyingyoupin.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hdz.vqdsnc.cn

[R50] awk 求和
来源：http://zni.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://chy.yanxiufei.cn

[R51] 排序去重取前几
来源：http://hpc.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qcm.yangfankeji.com

[R52] 统计行数
来源：http://nvn.aizwys.cn

wc -l a.txt
来源：http://uen.cheryme.top

[R53] 查看文件头与实时尾
来源：http://vuv.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vdy.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://tbf.hfpthk.cn

diff a.txt b.txt
来源：http://vwq.sjlbkw.cn

[R55] 压缩与解压
来源：http://idr.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://euq.bbcook.cn

[R56] 远程拷贝
来源：http://hcz.sjlbkw.cn

scp file user@host:/path/
来源：http://eac.svipenyu.cn

[R57] 远程执行命令
来源：http://ghy.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://vhy.yanxiufei.cn

[R58] 下载文件
来源：http://xiv.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tbf.xinyue.icu

[R59] 发 POST JSON
来源：http://ozk.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vun.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://ktx.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://twk.jinqigfzy.top

[R61] 磁盘占用
来源：http://avt.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://iiu.yongpay.top

[R62] 找最占空间的文件
来源：http://yeh.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://qbu.tianlin.xyz

[R63] 内存与进程
来源：http://lrk.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://nsh.zdqjudy.top

[R64] 结束进程
来源：http://ljd.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://dxe.vqdsnc.cn

[R65] 查看端口占用
来源：http://urv.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tyq.jinqigufen.top

[R66] 定时任务
来源：http://nvb.hnqzz.top

crontab -e;  crontab -l
来源：http://odb.daxiang520.top

[R67] 生成随机十六进制串
来源：http://wui.fzhhl.top

openssl rand -hex 16
来源：http://rnj.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://uzp.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://phw.nanxinkj.top

[R69] 生成随机密码
来源：http://ufo.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://bgp.fehbvm.com

[R70] 时间戳与互转
来源：http://aov.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://rpx.ybcxt.top

[R71] 日期格式化
来源：http://via.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://scu.yuxming.cn

[R72] 等待端口就绪
来源：http://xyy.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ftk.yj20258.top

[R73] 分割大日志
来源：http://twr.jqgfzy.top

split -l 1000 big.log part_
来源：http://hzy.hnqzz.top

[R74] 批量重命名
来源：http://ywu.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fhq.ppjwa.cn

[R75] 导出环境变量
来源：http://equ.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://vji.xuanzx.com

[R76] 使用临时文件
来源：http://duv.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ixo.jinqigfzy.top

[R77] 读取用户输入
来源：http://sru.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://wyu.jinqigfzy.top

[R78] 交互式菜单
来源：http://cui.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jnp.birdmap.top

[R79] 解析命令行选项
来源：http://sja.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pea.hcnkem.com

[R80] 查看脚本执行耗时
来源：http://brs.tarul.cn

time ./run.sh
来源：http://jaf.svipenyu.cn

================================================================================
来源：http://ivl.sjlbkw.cn

S. C / C++ 专题
来源：http://ipr.shanyushiyangkeji.top

================================================================================
来源：http://zgf.nanxuanxn.top

[S01] C：Hello World
来源：http://eid.yuanzhike.top

#include <stdio.h>
来源：http://jar.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fup.vehdjk.com

[S02] C：变量与格式化输出
来源：http://odt.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://chf.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://fxq.pycfn.com

int x; scanf("%d", &x);
来源：http://vau.cdnleiting.top

[S04] C：字符串复制
来源：http://jwi.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://hen.xylfe.cn

[S05] C：字符串长度
来源：http://kza.daxiang520.top

strlen(s)
来源：http://ldn.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://nnp.smart0.xyz

strcmp(a, b) == 0
来源：http://zzh.aibaodan.cn

[S07] C：数组遍历求和
来源：http://wck.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yao.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://nld.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ajc.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://kes.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zed.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://fjt.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://ezo.ydjk.org.cn

[S11] C：逐行读文件
来源：http://ojz.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://jbg.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://shb.gotoacloud.top

fclose(f);
来源：http://bem.hysaishi.cn

[S12] C：写文件
来源：http://nsp.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fze.wangdashe.top

[S13] C：宏定义
来源：http://dyg.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hmp.sjlbkw.cn

[S14] C：枚举
来源：http://qbj.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://qwg.zdbjq.cn

[S15] C：类型转换
来源：http://khw.andypj.xyz

(double) a / b
来源：http://uao.andypj.xyz

[S16] C：位操作置位
来源：http://ovs.zhiwuduotai.top

x |= (1 << 3);
来源：http://amg.yvedp.cn

[S17] C：安全拼接字符串
来源：http://reo.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nbq.cashguo.top

[S18] C：命令行参数
来源：http://kub.fzhhl.top

int main(int argc, char **argv)
来源：http://knc.aibaodan.cn

[S19] C：快速排序
来源：http://yes.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://ihi.tian-w.cn

[S20] C：二分查找
来源：http://wqx.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fpk.dianchejie.cn

[S21] C：字符类别判断
来源：http://hrj.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nsl.vehdjk.com

[S22] C：字符串转数字
来源：http://rrc.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://vyo.shangyingyoupin.top

[S23] C：随机数
来源：http://tbi.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://izn.gotoacloud.top

[S24] C：获取本地时间
来源：http://qmi.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tii.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://bzg.zdqjudy.top

memcpy(dst, src, n);
来源：http://dut.daria6918.cn

[S26] C：内存清零
来源：http://egi.fktsv.cn

memset(a, 0, sizeof a);
来源：http://ytp.fanxiaobao.xyz

[S27] C：定义常量
来源：http://jdv.yj20258888.top

const double PI = 3.14159;
来源：http://nxb.zhengqikj.top

[S28] C：静态变量
来源：http://xed.jqgufenzy.top

static int counter = 0;
来源：http://qlh.hammf.cn

[S29] C：变参函数
来源：http://tqw.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oat.yj20258888.top

[S30] C：头文件保护
来源：http://jqr.ivvv.top

#ifndef X_H
来源：http://uwz.yueranfly.top

#define X_H
来源：http://dku.zhongyouzk.top

#endif
来源：http://ntg.kuanghao11.cn

[S31] C++：Hello World
来源：http://koa.chenjidiqi.icu


<!-- 参考信息 -->