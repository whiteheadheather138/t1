代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mnk.haohaochexian.top

[Q58] 累计求和
来源：http://arc.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wsg.svipenyu.cn

[Q59] 分组内累计
来源：http://bch.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fmy.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://wpq.zdbjq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gzt.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lzr.epnwcf.com

[Q61] 移动平均
来源：http://uel.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ekf.hesvh.cn

[Q62] 分组占比
来源：http://iju.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sjo.jyoumei.cn

[Q63] 开启事务
来源：http://dhc.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fkc.guannengcc.top

[Q64] 提交事务
来源：http://lzp.haohaochexian.top

COMMIT;
来源：http://opw.chenjidiqi.icu

[Q65] 回滚事务
来源：http://tvs.ywan-chungtsiang.top

ROLLBACK;
来源：http://thg.zycfv.cn

[Q66] 行锁查询
来源：http://sdj.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://heo.xylfe.cn

[Q67] 设置隔离级别
来源：http://lju.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lhb.9152youxi.cn

[Q68] 保存点
来源：http://yak.bbcook.cn

SAVEPOINT sp1;
来源：http://pjr.jqgfzy.top

ROLLBACK TO sp1;
来源：http://ldi.dashuyun.cn

[Q69] 查看执行计划
来源：http://ecp.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tsx.jinqigfzy.top

[Q70] 更新统计信息
来源：http://xdy.yanxiufei.cn

ANALYZE TABLE users;
来源：http://tgp.jinqigufen.top

[Q71] 查看建表语句
来源：http://vax.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jqb.mhx1999.top

[Q72] 查看索引
来源：http://evf.zhengqikj.top

SHOW INDEX FROM users;
来源：http://bhl.feifeiyinyue.top

[Q73] 查看表状态
来源：http://lad.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://jwc.fzhhl.top

[Q74] 强制使用索引
来源：http://srt.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fif.yonumen.top

[Q75] 日期格式化
来源：http://vya.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vmp.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ioc.shangyingyoupin.top

[Q76] 按天统计
来源：http://zbp.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rrt.sweek.top

[Q77] 时间加减
来源：http://yzv.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://isi.zhoulong.xyz

[Q78] 当前时间
来源：http://edz.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cod.ehwqpu.com

[Q79] 字符串拼接
来源：http://cqo.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hkr.jinqigufen.top

[Q80] 字符串截取
来源：http://itd.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://drl.yuxming.cn

[Q81] 字符串替换
来源：http://bpn.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ftq.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://tej.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bmw.feifeiyinyue.top

[Q83] 大小写转换
来源：http://yvp.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mmi.52xcode.cn

[Q84] 去除首尾空格
来源：http://suh.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://yzr.ehwqpu.com

[Q85] 数值取整
来源：http://xfj.yanxiufei.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zyx.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://ano.mhx1999.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fsk.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://kus.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dpo.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://tug.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kox.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tgh.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://sve.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://swx.9152youxi.cn

[Q90] 生成序号列
来源：http://aie.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ovv.xingfuxueyuan.xyz

================================================================================
来源：http://wcs.jyoumei.cn

R. Bash 专题
来源：http://ots.c1oappe.top

================================================================================
来源：http://ynn.dashuyun.cn

[R01] shebang 与严格模式
来源：http://oda.guowangkeji.top

#!/usr/bin/env bash
来源：http://mew.chenjidiqi.icu

set -euo pipefail
来源：http://cts.zhengqikj.top

[R02] 变量赋值与使用
来源：http://qxj.ydjk.org.cn

name="Tom"; echo "$name"
来源：http://fxo.aizwys.cn

[R03] 只读变量
来源：http://vzn.hysaishi.cn

readonly PI=3.14
来源：http://yza.fktsv.cn

[R04] 位置参数
来源：http://arv.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ill.yj20258888.top

[R05] 参数默认值
来源：http://otb.jinqigfzy.top

name="${1:-default}"
来源：http://ixo.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://qyj.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://shh.aibaodan.cn

[R07] if 判断文件
来源：http://xbv.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://weu.c1oappe.top

[R08] 数值比较
来源：http://bpy.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jvt.9152youxi.cn

[R09] 字符串比较
来源：http://ywg.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xxn.zhongyouzk.top

[R10] 正则匹配
来源：http://smn.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://utr.hesvh.cn

[R11] case 多分支
来源：http://abg.quarkkingdee.top

case "$1" in
来源：http://edr.ydjk.org.cn

start) echo "启动" ;;
来源：http://wvy.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://qgy.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://qgl.316326.xyz

esac
来源：http://jqw.hnqzz.top

[R12] for 遍历文件
来源：http://kbq.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://rqx.vehdjk.com

[R13] for 计数循环
来源：http://oce.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://uez.ehwqpu.com

[R14] C 风格 for
来源：http://uue.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://obe.vehdjk.com

[R15] while 逐行读文件
来源：http://opp.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://met.ydzc1.top

[R16] until 等待条件
来源：http://fgl.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jcy.guowangkeji.top

[R17] 数组定义与取值
来源：http://dkz.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://jan.sjlbkw.cn

[R18] 遍历数组
来源：http://mmg.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yxa.yj202588.top

[R19] 数组长度
来源：http://qcj.yangfankeji.com

echo "${#arr[@]}"
来源：http://tbl.gogol.net.cn

[R20] 关联数组（字典）
来源：http://toi.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fcj.chenzaomai.com

[R21] 字符串长度
来源：http://fme.sweek.top

echo "${#s}"
来源：http://jdl.cqqwz.cn

[R22] 截取子串
来源：http://acu.cheryme.top

echo "${s:0:5}"
来源：http://oos.yanxiufei.cn

[R23] 字符串替换
来源：http://oru.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jqd.ybcxt.top

[R24] 大小写转换
来源：http://qnh.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ges.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://cwn.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://kzp.hnqzz.top

[R26] 命令替换
来源：http://swl.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://vbw.hysaishi.cn

[R27] 算术展开
来源：http://lcx.52xcode.cn

echo $((1 + 2 * 3))
来源：http://fux.yonumen.top

[R28] 浮点运算
来源：http://ywd.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://eje.andypj.xyz

[R29] 定义函数
来源：http://osa.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://avh.kuanghao11.cn

[R30] 函数返回状态码
来源：http://vyq.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://nnh.jlsjyb.cn

[R31] 局部变量
来源：http://jyu.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://cjl.xinyue.icu

[R32] 参数个数校验
来源：http://ziw.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nkh.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://rij.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pky.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://nuk.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://vom.cqqwz.cn

[R35] 后台执行并等待
来源：http://psu.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ojg.zhengqikj.top

[R36] 并发执行多个任务
来源：http://rhh.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cdl.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://vtq.fanxiaobao.xyz

files=$(ls -1)
来源：http://rjp.wangshuangyany.cn

[R38] 管道串联
来源：http://yup.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://vnr.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://xko.ctjpmb.com

cmd > out.log 2>&1
来源：http://nlq.shuidangran.top

[R40] 追加写日志
来源：http://tgw.mhx1999.top

echo "log" >> out.log
来源：http://pja.yfazqb.com

[R41] 丢弃输出
来源：http://ihq.xinyue.icu

cmd >/dev/null 2>&1
来源：http://oya.zhoulong.xyz

[R42] 输入重定向
来源：http://jcl.zycfv.cn

wc -l < a.txt
来源：http://zjc.ivvv.top

[R43] 按名字查找文件
来源：http://yoh.hnqzz.top

find . -name "*.log" -type f
来源：http://ojw.birdmap.top

[R44] 按修改时间查找
来源：http://gbh.snrcjt.cn

find . -mtime -7 -type f
来源：http://dnn.bbcook.cn

[R45] 批量删除
来源：http://sxd.yvedp.cn

find . -name "*.tmp" -delete
来源：http://its.sxryk.cn

[R46] 递归替换文件内容
来源：http://eki.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ubc.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://vag.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kda.xinyue.icu

[R48] awk 取指定列
来源：http://zji.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://iwy.jinqigfzy.top

[R49] awk 带条件
来源：http://tkn.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zmj.ctjpmb.com

[R50] awk 求和
来源：http://ilm.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bfr.dashuyun.cn

[R51] 排序去重取前几
来源：http://sxq.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://osx.gotoacloud.top

[R52] 统计行数
来源：http://dqw.shangyingyoupin.top

wc -l a.txt
来源：http://tjw.yangfankeji.com

[R53] 查看文件头与实时尾
来源：http://bsn.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ald.yvedp.cn

[R54] 比较两个文件
来源：http://mbx.cqqwz.cn

diff a.txt b.txt
来源：http://ckn.yongpay.top

[R55] 压缩与解压
来源：http://rdq.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://woi.ctjpmb.com

[R56] 远程拷贝
来源：http://vrj.sufxvd.cn

scp file user@host:/path/
来源：http://pfd.jlsjyb.cn

[R57] 远程执行命令
来源：http://gyq.sxryk.cn

ssh user@host 'uptime'
来源：http://ozy.yfazqb.com

[R58] 下载文件
来源：http://ihb.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hpo.kuanghao11.cn

[R59] 发 POST JSON
来源：http://iys.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ehg.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://ukd.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jzq.tarul.cn

[R61] 磁盘占用
来源：http://nfc.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://pyh.hammf.cn

[R62] 找最占空间的文件
来源：http://yqr.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://ygd.jiagoushi.top

[R63] 内存与进程
来源：http://nqa.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://qwx.jinqigufen.top

[R64] 结束进程
来源：http://akl.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://lyj.yj20258888.top

[R65] 查看端口占用
来源：http://imt.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vqh.xinyue.icu

[R66] 定时任务
来源：http://xjb.yuxming.cn

crontab -e;  crontab -l
来源：http://srn.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://dmf.tian-w.cn

openssl rand -hex 16
来源：http://xgo.hcnkem.com

[R68] 计算文件校验值
来源：http://lqy.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bvk.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://emf.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://ujj.zhijiandao.cn

[R70] 时间戳与互转
来源：http://jdg.52xcode.cn

date +%s;  date -d @1700000000
来源：http://otw.daria6918.cn

[R71] 日期格式化
来源：http://dnb.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oqm.hnqzz.top

[R72] 等待端口就绪
来源：http://hvn.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kez.zhongyouzk.top

[R73] 分割大日志
来源：http://tee.yvedp.cn

split -l 1000 big.log part_
来源：http://bfg.smart0.xyz

[R74] 批量重命名
来源：http://kaf.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ibs.redwolf501.top

[R75] 导出环境变量
来源：http://qgw.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://eys.andypj.xyz

[R76] 使用临时文件
来源：http://rzu.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bwo.yonumen.top

[R77] 读取用户输入
来源：http://uuq.aizwys.cn

read -rp "请输入: " ans
来源：http://isi.hnqzz.top

[R78] 交互式菜单
来源：http://asz.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sgl.zdbjq.cn

[R79] 解析命令行选项
来源：http://puk.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hum.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://jcg.shanyushiyangtech.top

time ./run.sh
来源：http://dlu.shzxlz.cn

================================================================================
来源：http://kdy.shuidangran.top

S. C / C++ 专题
来源：http://xtt.zhaomingkeji.xyz

================================================================================
来源：http://due.svipenyu.cn

[S01] C：Hello World
来源：http://fqu.sysykeji.top

#include <stdio.h>
来源：http://xtm.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kua.xziqi.cn

[S02] C：变量与格式化输出
来源：http://zea.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://zio.316326.xyz

[S03] C：读入整数
来源：http://syv.c1oappe.top

int x; scanf("%d", &x);
来源：http://urc.havefunace.top

[S04] C：字符串复制
来源：http://lea.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tec.vqdsnc.cn

[S05] C：字符串长度
来源：http://ejr.zhaomingkeji.xyz

strlen(s)
来源：http://mpy.jianghu66.top

[S06] C：字符串比较
来源：http://dlc.nanxinkj.top

strcmp(a, b) == 0
来源：http://lqu.gotoacloud.top

[S07] C：数组遍历求和
来源：http://pps.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hme.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://ucu.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mqs.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://yll.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://prq.sweek.top

[S10] C：指针与解引用
来源：http://obr.daxiang520.top

int *p = &a;  *p = 5;
来源：http://hew.xziqi.cn

[S11] C：逐行读文件
来源：http://uky.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://pfi.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nts.daxiang520.top

fclose(f);
来源：http://vdv.c1oappe.top

[S12] C：写文件
来源：http://twf.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rkk.jiagoushi.top

[S13] C：宏定义
来源：http://lhs.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vzl.316326.xyz

[S14] C：枚举
来源：http://oxb.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://hto.tanke756.top

[S15] C：类型转换
来源：http://oyl.316326.xyz

(double) a / b
来源：http://qed.feifeiyinyue.top

[S16] C：位操作置位
来源：http://hom.nanxuanxn.top

x |= (1 << 3);
来源：http://liy.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://byz.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iny.uphjek.com

[S18] C：命令行参数
来源：http://pjz.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://oba.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://jmx.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ypi.tianlin.xyz

[S20] C：二分查找
来源：http://ziu.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bzk.fehbvm.com

[S21] C：字符类别判断
来源：http://pwr.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tdg.yangfankeji.com

[S22] C：字符串转数字
来源：http://kmm.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://qqj.jinyuanbaomall.cn

[S23] C：随机数
来源：http://oqv.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uhr.kuanghao11.cn

[S24] C：获取本地时间
来源：http://yle.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nxr.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://lwn.nwbrower.top

memcpy(dst, src, n);
来源：http://qkv.zycfv.cn

[S26] C：内存清零
来源：http://twq.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://tze.zdbjq.cn

[S27] C：定义常量
来源：http://tpi.xuetiantiany.cn

const double PI = 3.14159;
来源：http://lly.chenlongwang.top

[S28] C：静态变量
来源：http://eqa.ppjwa.cn


<!-- 参考信息 -->